# Rules

This section outlines the rules applied within this checkstyle file and why they have been configured.

| Rule                               | Configuration | Description |
| ---------------------------------- | ------------- | ----------- |
| [AbbreviationAsWordInName](https://checkstyle.sourceforge.io/checks/naming/abbreviationaswordinname.html#AbbreviationAsWordInName)  | N/A | |
| [AbstractClassName](https://checkstyle.sourceforge.io/checks/naming/abstractclassname.html#AbstractClassName)        | N/A | |
| [AnonInnerLength](https://checkstyle.sourceforge.io/checks/sizes/anoninnerlength.html#AnonInnerLength)               | N/A | |
| [AnnotationLocation](https://checkstyle.sourceforge.io/checks/annotation/annotationlocation.html#AnnotationLocation) | N/A | |
| [AvoidNestedBlocks](https://checkstyle.sourceforge.io/checks/blocks/avoidnestedblocks.html#AvoidNestedBlocks)        | N/A | |
| [ArrayTrailingComma](https://checkstyle.sourceforge.io/checks/coding/arraytrailingcomma.html#ArrayTrailingComma)     | N/A | |
| [ArrayTypeStyle](https://checkstyle.sourceforge.io/checks/misc/arraytypestyle.html#ArrayTypeStyle)                   | N/A | |
| [AvoidDoubleBraceInitialization](https://checkstyle.sourceforge.io/checks/coding/avoiddoublebraceinitialization.html#AvoidDoubleBraceInitialization) | N/A | |
| [AvoidNoArgumentSuperConstructorCall](https://checkstyle.sourceforge.io/checks/coding/avoidnoargumentsuperconstructorcall.html#AvoidNoArgumentSuperConstructorCall) | N/A | |
| [AvoidStarImport](https://checkstyle.sourceforge.io/checks/imports/avoidstarimport.html#AvoidStarImport)             | N/A | It is each for projects to pull in multiple libraries and so have multiple classes with the same name on the classpath. The requirement for explicitly importing each class allows developers to see when they have imported a class from the wrong library. |
| [CovariantEquals](https://checkstyle.sourceforge.io/checks/coding/covariantequals.html#CovariantEquals)              | N/A | |
| [CommentsIndentation](https://checkstyle.sourceforge.io/checks/misc/commentsindentation.html#CommentsIndentation)    | N/A | |
| [CatchParameterName](https://checkstyle.sourceforge.io/checks/naming/catchparametername.html#CatchParameterName)     | N/A | |
| [ClassTypeParameterName](https://checkstyle.sourceforge.io/checks/naming/classtypeparametername.html#ClassTypeParameterName)        | N/A | |
| [ConstantName](https://checkstyle.sourceforge.io/checks/naming/constantname.html#ConstantName)                       | N/A | |
| [CyclomaticComplexity](https://checkstyle.sourceforge.io/checks/metrics/cyclomaticcomplexity.html#CyclomaticComplexity)             | N/A | |
| [DeclarationOrder](https://checkstyle.sourceforge.io/checks/coding/declarationorder.html#DeclarationOrder)           | N/A | |
| [DefaultComesLast](https://checkstyle.sourceforge.io/checks/coding/defaultcomeslast.html#DefaultComesLast)           | N/A | |
| [EmptyStatement](https://checkstyle.sourceforge.io/checks/coding/emptystatement.html#EmptyStatement)                 | N/A | |
| [EqualsAvoidNull](https://checkstyle.sourceforge.io/checks/coding/equalsavoidnull.html#EqualsAvoidNull)              | N/A | |
| [EqualsHashCode](https://checkstyle.sourceforge.io/checks/coding/equalshashcode.html#EqualsHashCode)                 | N/A | |
| [EmptyBlock](https://checkstyle.sourceforge.io/checks/blocks/emptyblock.html#EmptyBlock)                             | * LITERAL_WHILE <br/> * LITERAL_TRY <br/> * LITERAL_CATCH <br/> * LITERAL_FINALLY <br/> * LITERAL_DO <br/> * LITERAL_IF <br/> * LITERAL_ELSE <br/> * LITERAL_FOR <br/> * INSTANCE_INIT <br/> * STATIC_INIT <br/> * LITERAL_SWITCH <br/> * LITERAL_SYNCHRONIZED <br/> * LITERAL_CASE <br/> * ARRAY_INIT | |
| [EmptyCatchBlock](https://checkstyle.sourceforge.io/checks/blocks/emptycatchblock.html#EmptyCatchBlock)              | N/A | |
| [EmptyForInitializerPad](https://checkstyle.sourceforge.io/checks/whitespace/emptyforinitializerpad.html#EmptyForInitializerPad)    | N/A | |
| [EmptyForIteratorPad](https://checkstyle.sourceforge.io/checks/whitespace/emptyforiteratorpad.html#EmptyForIteratorPad)             | N/A | |
| [ExecutableStatementCount](https://checkstyle.sourceforge.io/checks/sizes/executablestatementcount.html#ExecutableStatementCount)   | N/A | |
| [FinalParameters](https://checkstyle.sourceforge.io/checks/misc/finalparameters.html#FinalParameters)                | N/A | |
| [FileLength](https://checkstyle.sourceforge.io/checks/sizes/filelength.html#FileLength)                              | * max="2000" | |
| [FileTabCharacter](https://checkstyle.sourceforge.io/checks/whitespace/filetabcharacter.html#FileTabCharacter)       | N/A | |
| [FinalClass](https://checkstyle.sourceforge.io/checks/design/finalclass.html#FinalClass)                             | N/A | |
| [FinalLocalVariable](https://checkstyle.sourceforge.io/checks/coding/finallocalvariable.html#FinalLocalVariable)     | * VARIABLE_DEF <br/> * PARAMETER_DEF | If a variable is set and not reassigned we want to define it as final. This helps identify objects which are changed within a function/class and those which are static. |
| [GenericWhitespace](https://checkstyle.sourceforge.io/checks/whitespace/genericwhitespace.html#GenericWhitespace)    | N/A | |
| [HideUtilityClassConstructor](https://checkstyle.sourceforge.io/checks/design/hideutilityclassconstructor.html#HideUtilityClassConstructor)          | N/A | |
| [HiddenField](https://checkstyle.sourceforge.io/checks/coding/hiddenfield.html#HiddenField)                          | N/A | |
| [IllegalInstantiation](https://checkstyle.sourceforge.io/checks/coding/illegalinstantiation.html#IllegalInstantiation)              | N/A | |
| [IllegalCatch](https://checkstyle.sourceforge.io/checks/coding/illegalcatch.html#IllegalCatch)                       | N/A | |
| [IllegalThrows](https://checkstyle.sourceforge.io/checks/coding/illegalthrows.html#IllegalThrows)                    | N/A | |
| [InnerAssignment](https://checkstyle.sourceforge.io/checks/coding/innerassignment.html#InnerAssignment)              | N/A | |
| [InnerTypeLast](hhttps://checkstyle.sourceforge.io/checks/design/innertypelast.html#InnerTypeLastttps)               | N/A | |
| [InterfaceIsType](https://checkstyle.sourceforge.io/checks/design/interfaceistype.html#InterfaceIsType)              | N/A | |
| [Indentation](https://checkstyle.sourceforge.io/checks/misc/indentation.html#Indentation) | * basicOffset="2" <br/> * caseIndent="2" <br/> * throwsIndent="2" <br/> * arrayInitIndent="2" <br/> * lineWrappingIndentation="2"   | |
| [IllegalImport](https://checkstyle.sourceforge.io/checks/imports/illegalimport.html#IllegalImport)                   | N/A | |
| [InvalidJavadocPosition](https://checkstyle.sourceforge.io/checks/javadoc/invalidjavadocposition.html#InvalidJavadocPosition)       | N/A | |
| [JavadocContentLocation](https://checkstyle.sourceforge.io/checks/javadoc/javadoccontentlocation.html#JavadocContentLocation)       | N/A | |
| [JavadocMethod](https://checkstyle.sourceforge.io/checks/javadoc/javadocmethod.html#JavadocMethod)                   | N/A | |
| [JavadocMissingLeadingAsterisk](https://checkstyle.sourceforge.io/checks/javadoc/javadocmissingleadingasterisk.html#JavadocMissingLeadingAsterisk)   | N/A | |
| [JavadocStyle](https://checkstyle.sourceforge.io/checks/javadoc/javadocstyle.html#JavadocStyle)                      | N/A | |
| [JavadocTagContinuationIndentation](https://checkstyle.sourceforge.io/checks/javadoc/javadoctagcontinuationindentation.html#JavadocTagContinuationIndentation) | * offset="2" | |
| [JavadocVariable](https://checkstyle.sourceforge.io/checks/javadoc/javadocvariable.html#JavadocVariable)             | N/A | |
| [LeftCurly](https://checkstyle.sourceforge.io/checks/blocks/leftcurly.html#LeftCurly)                                | N/A | |
| [LambdaBodyLength](https://checkstyle.sourceforge.io/checks/sizes/lambdabodylength.html#LambdaBodyLength)            | N/A | |
| [LineLength](https://checkstyle.sourceforge.io/checks/sizes/linelength.html#LineLength)                              | * max="120" | Historically 80 characters was used to ensure an entire line of code was visible on a screen, screens have gotten larger and high resolution and so ~200 characters are now visible on a single line. <br/> We set the limit to 120 characters to balance the ability to use larger names |
| [LocalFinalVariableName](https://checkstyle.sourceforge.io/checks/naming/localfinalvariablename.html#LocalFinalVariableName) | N/A | |
| [LambdaParameterName](https://checkstyle.sourceforge.io/checks/naming/lambdaparametername.html#LambdaParameterName)  | N/A | |
| [LocalVariableName](https://checkstyle.sourceforge.io/checks/naming/localvariablename.html#LocalVariableName)        | N/A | |
| [MagicNumber](https://checkstyle.sourceforge.io/checks/coding/magicnumber.html#MagicNumber)                          | N/A | When working at a low technical level it is common to assign meaning to integer values. This can result in a situation where a conditional is based on a numeric value and there are many legacy codebases with references such as if (x == 10). This requires developers to assign the number ot a variable and combined with the variable name length rules should ensure there is context to the numeric value (e.g. final int NEW_LINE = 43; if (x == NEW_LINE )). |
| [MissingDeprecated](https://checkstyle.sourceforge.io/checks/annotation/missingdeprecated.html#MissingDeprecated)    | N/A | |
| [MissingOverride](https://checkstyle.sourceforge.io/checks/annotation/missingoverride.html#MissingOverride)          | N/A | |
| [MutableException](https://checkstyle.sourceforge.io/checks/design/mutableexception.html#MutableException)           | N/A | |
| [MissingCtor](https://checkstyle.sourceforge.io/checks/coding/missingctor.html#MissingCtor)                          | N/A | |
| [MissingSwitchDefault](https://checkstyle.sourceforge.io/checks/coding/missingswitchdefault.html#MissingSwitchDefault)              | N/A | |
| [ModifiedControlVariable](https://checkstyle.sourceforge.io/checks/coding/modifiedcontrolvariable.html#ModifiedControlVariable)     | N/A | |
| [MultipleStringLiterals](https://checkstyle.sourceforge.io/checks/coding/multiplestringliterals.html#MultipleStringLiterals)        | N/A | |
| [MultipleVariableDeclarations](https://checkstyle.sourceforge.io/checks/coding/multiplevariabledeclarations.html#MultipleVariableDeclarations) | N/A | |
| [MethodCount](https://checkstyle.sourceforge.io/checks/sizes/methodcount.html#MethodCount)                           | N/A | |
| [MethodLength](https://checkstyle.sourceforge.io/checks/sizes/methodlength.html#MethodLength)                        | * max="100 | Forces code to be split into descrete units, this stops giant methods which perform all operations forcing developers to break code out into logical chunks. |
| [MemberName](https://checkstyle.sourceforge.io/checks/naming/membername.html#MemberName)                             | N/A | |
| [MethodName](https://checkstyle.sourceforge.io/checks/naming/methodname.html#MethodName)                             | N/A | |
| [MethodTypeParameterName](https://checkstyle.sourceforge.io/checks/naming/methodtypeparametername.html#MethodTypeParameterName) | N/A | |
| [ModifierOrder](https://checkstyle.sourceforge.io/checks/modifier/modifierorder.html#ModifierOrder)                  | N/A | |
| [NoArrayTrailingComma](https://checkstyle.sourceforge.io/checks/coding/noarraytrailingcomma.html#NoArrayTrailingComma) | N/A | |
| [NeedBraces](https://checkstyle.sourceforge.io/checks/blocks/needbraces.html#NeedBraces)                             | * LITERAL_DO <br/> * LITERAL_ELSE <br/> * LITERAL_FOR <br/> *LITERAL_IF <br/> * LITERAL_WHILE <br/> * LITERAL_CASE | |
| [NoEnumTrailingComma](https://checkstyle.sourceforge.io/checks/coding/noenumtrailingcomma.html#NoEnumTrailingComma)  | N/A | |
| [NoLineWrap](https://checkstyle.sourceforge.io/checks/whitespace/nolinewrap.html#NoLineWrap)                         | * IMPORT <br/> * STATIC_IMPORT <br/> * PACKAGE_DEF | |
| [NoWhitespaceAfter](https://checkstyle.sourceforge.io/checks/whitespace/nowhitespaceafter.html#NoWhitespaceAfter)    | N/A | |
| [NPathComplexity](https://checkstyle.sourceforge.io/checks/metrics/npathcomplexity.html#NPathComplexity)             | N/A | |
| [NoCodeInFile](https://checkstyle.sourceforge.io/checks/misc/nocodeinfile.html#NoCodeInFile)                         | N/A | |
| [OneStatementPerLine](https://checkstyle.sourceforge.io/checks/coding/onestatementperline.html#OneStatementPerLine)  | N/A | |
| [OneTopLevelClass](https://checkstyle.sourceforge.io/checks/design/onetoplevelclass.html#OneTopLevelClass)           | N/A | |
| [OuterTypeNumber](https://checkstyle.sourceforge.io/checks/sizes/outertypenumber.html#OuterTypeNumber)               | N/A | |
| [OuterTypeFilename](https://checkstyle.sourceforge.io/checks/misc/outertypefilename.html#OuterTypeFilename)          | N/A | |
| [PackageDeclaration](https://checkstyle.sourceforge.io/checks/coding/packagedeclaration.html#PackageDeclaration)     | N/A | |
| [PackageName](https://checkstyle.sourceforge.io/checks/naming/packagename.html#PackageName)                          | N/A | |
| [ParameterName](https://checkstyle.sourceforge.io/checks/naming/parametername.html#ParameterName)                    | N/A | |
| [PatternVariableName](https://checkstyle.sourceforge.io/checks/naming/patternvariablename.html#PatternVariableName)  | N/A | |
| [ParameterNumber](https://checkstyle.sourceforge.io/checks/sizes/parameternumber.html#ParameterNumber)               | N/A | |
| [RecordComponentNumber](https://checkstyle.sourceforge.io/checks/sizes/recordcomponentnumber.html#RecordComponentNumber)            | N/A | |
| [RecordTypeParameterName](https://checkstyle.sourceforge.io/checks/naming/recordtypeparametername.html#RecordTypeParameterName)     | N/A | |
| [RightCurly](https://checkstyle.sourceforge.io/checks/blocks/rightcurly.html#RightCurly)                             | N/A | |
| [RequireThis](https://checkstyle.sourceforge.io/checks/coding/requirethis.html#RequireThis)                          | N/A | |
| [RedundantImport](https://checkstyle.sourceforge.io/checks/imports/redundantimport.html#RedundantImport)             | N/A | |
| [ReturnCount](https://checkstyle.sourceforge.io/checks/coding/returncount.html#ReturnCount)                          | N/A | Historically a lot of applications had dozens of return statements this created dozens of routes through a method which made understanding it very challanging. |
| [RedundantModifier](https://checkstyle.sourceforge.io/checks/modifier/redundantmodifier.html#RedundantModifier)      | N/A | |
| [RegexpSingleline](https://checkstyle.sourceforge.io/checks/regexp/regexpsingleline.html#RegexpSingleline)           | N/A | |
| [SimplifyBooleanExpression](https://checkstyle.sourceforge.io/checks/coding/simplifybooleanexpression.html#SimplifyBooleanExpression) | N/A | |
| [SimplifyBooleanReturn](https://checkstyle.sourceforge.io/checks/coding/simplifybooleanreturn.html#SimplifyBooleanReturn) | N/A | |
| [StringLiteralEquality](https://checkstyle.sourceforge.io/checks/coding/stringliteralequality.html#StringLiteralEquality) | N/A | |
| [SuperClone](https://checkstyle.sourceforge.io/checks/coding/superclone.html#SuperClone)                             | N/A | |
| [StaticVariableName](https://checkstyle.sourceforge.io/checks/naming/staticvariablename.html#StaticVariableName)     | N/A | |
| [TypeName](https://checkstyle.sourceforge.io/checks/naming/typename.html#TypeName)                                   | N/A | |
| [TodoComment](https://checkstyle.sourceforge.io/checks/misc/trailingcomment.html#TrailingComment)                    | N/A | |
| [TrailingComment](https://checkstyle.sourceforge.io/checks/misc/trailingcomment.html#TrailingComment)                | N/A | |
| [Translation](https://checkstyle.sourceforge.io/checks/misc/translation.html#Translation)                            | N/A | |
| [ThrowsCount](https://checkstyle.sourceforge.io/checks/design/throwscount.html#ThrowsCount)                          | N/A | |
| [UnnecessaryParentheses](https://checkstyle.sourceforge.io/checks/coding/unnecessaryparentheses.html#UnnecessaryParentheses) | N/A | |
| [UnnecessarySemicolonAfterOuterTypeDeclaration](https://checkstyle.sourceforge.io/checks/coding/unnecessarysemicolonafteroutertypedeclaration.html#UnnecessarySemicolonAfterOuterTypeDeclaration)    | N/A | |
| [UnnecessarySemicolonAfterTypeMemberDeclaration](https://checkstyle.sourceforge.io/checks/coding/unnecessarysemicolonaftertypememberdeclaration.html#UnnecessarySemicolonAfterTypeMemberDeclaration) | N/A | |
| [UnnecessarySemicolonInEnumeration](https://checkstyle.sourceforge.io/checks/coding/unnecessarysemicoloninenumeration.html#UnnecessarySemicolonInEnumeration) | N/A | |
| [UnnecessarySemicolonInTryWithResources](https://checkstyle.sourceforge.io/checks/coding/unnecessarysemicolonintrywithresources.html#UnnecessarySemicolonInTryWithResources) | N/A | |
| [UnusedImports](https://checkstyle.sourceforge.io/checks/imports/unusedimports.html#UnusedImports)                   | N/A | |
| [UnusedLocalVariable](https://checkstyle.sourceforge.io/checks/coding/unusedlocalvariable.html#UnusedLocalVariable)  | N/A | |
| [UncommentedMain](https://checkstyle.sourceforge.io/checks/misc/uncommentedmain.html#UncommentedMain)                | N/A | |
| [UpperEll](https://checkstyle.sourceforge.io/checks/misc/upperell.html#UpperEll)                                     | N/A | |
| [UniqueProperties](https://checkstyle.sourceforge.io/checks/misc/uniqueproperties.html#UniqueProperties)             | N/A | |
| [VisibilityModifier](https://checkstyle.sourceforge.io/checks/design/visibilitymodifier.html#VisibilityModifier)     | N/A | |
| [VariableDeclarationUsageDistance](https://checkstyle.sourceforge.io/checks/coding/variabledeclarationusagedistance.html#VariableDeclarationUsageDistance) | allowedDistance="10" | |
