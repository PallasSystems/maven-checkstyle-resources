# Overview

This project was created to ensure a consistent set of Checkstyle (Java formatting) rules are used accross all Pallas Systems projects. A checkstyle file has been uploaded into the central repository so it can be retrieved via the build system and so embedded into the build process directly.

## Maven

This section outlines how you can use Maven to retrieve the rule file and run Checkstyle on your project.

### Commands

It is possible to call Maven plugins from the command line, the following will retrieve the Checkstyle rule file and then run the Checkstyle plugin

```bash

mvn --batch-mode org.apache.maven.plugins:maven-dependency-plugin:3.6.1:get -Dartifact=uk.pallas.systems.site:checkstyle:${project.version}:xml:checkstyle

mvn --batch-mode org.apache.maven.plugins:maven-checkstyle-plugin:3.3.0:checkstyle-aggregate -Dcheckstyle.config.location=~/.m2/repository/uk/pallas/systems/site/checkstyle/${project.version}/checkstyle-${project.version}-checkstyle.xml

```

### Super POM

The easiest way to embed the checkstyle rules into your project is to add the Pallas Systems Parent POM to your project like so:

```xml
<parent>
  <groupId>uk.pallas.systems</groupId>
  <artifactId>parent</artifactId>
  <version>1.0.3</version>
</parent>
```

### POM Configuration

You may not want to use the Pallas Systems Parent POM, below is the POM configuration the parent project uses to embed Checkstyle into the project build process. THis works by including the checkstyle library as a dependency of the checkstyle plugin, this places the rules file on the Java Classpath, the reporting section lists the path you can expect to find the rules file.

```xml
<properties>
  <!-- Used to get the Site files into the right structure, while also being readable in an SCM. -->
  <maven-checkstyle-plugin.version>3.3.1</maven-checkstyle-plugin.version>
  <uk.pallas.systems.site.version>0.0.5</uk.pallas.systems.site.version>
</properties>

<build>
  <pluginManagement>
    <plugins>
      <plugin>
        <groupId>org.apache.maven.plugins</groupId>
        <artifactId>maven-checkstyle-plugin</artifactId>
        <version>${maven-checkstyle-plugin.version}</version>
        <configuration>
          <configLocation>Checkstyle.xml</configLocation>
          <consoleOutput>true</consoleOutput>
        </configuration>
        <dependencies>
          <dependency>
            <groupId>uk.pallas.systems.site</groupId>
            <artifactId>checkstyle</artifactId>
            <version>${project.version}</version>
          </dependency>
        </dependencies>
      </plugin>
    </plugins>
  </pluginManagement>
</build>

<reporting>
  <plugins>
    <plugin>
      <groupId>org.apache.maven.plugins</groupId>
      <artifactId>maven-checkstyle-plugin</artifactId>
      <reportSets>
        <reportSet>
          <reports>
            <report>checkstyle-aggregate</report>
          </reports>
        </reportSet>
      </reportSets>
    </plugin>
  </plugins>
</reporting>
```

## GitHub Actions

The below is an extract for building a project with checks for

```yml
- name: Checkstyle
  run: mvn --batch-mode --settings /tmp/java_maven_settings.xml org.apache.maven.plugins:maven-checkstyle-plugin:3.3.0:checkstyle-aggregate
  env:
    GITHUB_USER: ${{ secrets.SCM_USER }}
    GITHUB_TOKEN: ${{ secrets.SCM_TOKEN }}
    GPG_KEY_ID: ${{ secrets.GPG_PRIVATE_KEYNAME }}
    GPG_PASSPHRASE: ${{ secrets.GPG_PRIVATE_KEY_PASSPHRASE }}

- name: Checkstyle Annotation
  uses: jwgmeligmeyling/checkstyle-github-action@master
  with:
    path: "**/checkstyle-result.xml"
```
