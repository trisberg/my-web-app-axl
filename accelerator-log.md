# Accelerator Log

## Options
```json
{
  "nativeBuild" : true,
  "bsGitBranch" : "main",
  "includeBuildToolWrapper" : true,
  "javaVersion" : "21",
  "bsGitRepository" : "github.com?owner=trisberg&repo=my-web-app-axl",
  "buildTool" : "gradle",
  "ide" : "intellij",
  "includeDevContainer" : false,
  "projectName" : "my-web-app-axl"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Exclude, GeneratorValidationTransform, UniquePath)
┃ ┏ engine.transformations[0] (Exclude)
┃ ┃  Info Will exclude [accelerator.yaml, accelerator.axl]
┃ ┃ Debug .gitignore didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug .tanzuignore didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug LICENSE didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug README-native.md didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug README.md didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug Tiltfile didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug Tiltfile_gradle_intellij didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug Tiltfile_gradle_vscode didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug accelerator.axl matched [accelerator.yaml, accelerator.axl] -> excluded
┃ ┃ Debug accelerator.yaml matched [accelerator.yaml, accelerator.axl] -> excluded
┃ ┃ Debug build.gradle.kts didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug pom.xml didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug settings.gradle didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug catalog/catalog-info.yaml didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug config/workload-native.yaml didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug config/workload.yaml didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug src/main/resources/application.yml didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug src/main/java/com/example/springboot/Application.java didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug src/main/java/com/example/springboot/HelloController.java didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┗ Debug src/test/java/com/example/springboot/HelloControllerTest.java didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┏ ┏ engine.transformations[1].validated (Chain)
┃ ┃ ┃  Info Running Chain(IfElse, IfElse, ApplyTo, ApplyTo, ApplyTo, ApplyTo, IfElse, Merge, UniquePath, Provenance)
┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0] (IfElse)
┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1] (IfElse)
┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[1].then (Chain)
┃ ┃ ┃ ┃  Info Running Chain(ApplyTo, IfElse, IfElse, Merge)
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].then.transformations[0].apply (ReplaceText)
┃ ┃ ┃ ┃ ┗  Info Will replace [tanzu-java-web-app->my-web-app-axl]
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].then.transformations[1] (IfElse)
┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[1].then.transformations[1].then (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Exclude, RewritePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].then.transformations[1].then.transformations[0] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [Tiltfile, Tiltfile_gradle_vscode]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README-native.md didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [Tiltfile, Tiltfile_gradle_vscode] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile_gradle_intellij didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile_gradle_vscode matched [Tiltfile, Tiltfile_gradle_vscode] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle.kts didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-native.yaml didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yml didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/Application.java didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/HelloController.java didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/springboot/HelloControllerTest.java didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┗ Debug settings.gradle didn't match [Tiltfile, Tiltfile_gradle_vscode] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].then.transformations[1].then.transformations[1] (RewritePath)
┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'Tiltfile_gradle_intellij' matched 'Tiltfile_gradle_intellij' with groups {g0=Tiltfile_gradle_intellij} and was rewritten to 'Tiltfile'
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].then.transformations[2] (IfElse)
┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].then.transformations[3] (Merge)
┃ ┃ ┃ ┃ ┃  Info Running Merge(Exclude, InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].then.transformations[3].sources[0] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README-native.md didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle.kts didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-native.yaml didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yml didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/Application.java didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/HelloController.java didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/springboot/HelloControllerTest.java didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┗ Debug settings.gradle didn't match [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].then.transformations[3].sources[1] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].then.transformations[3].sources[1].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[1].then.transformations[3].sources[1].validated.delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].then.transformations[3].sources[1].validated.delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].then.transformations[3].sources[1].validated.delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#includeBuildToolWrapper) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[1].then.transformations[3].sources[1].validated.delegate.transformations[0].sources[0].delegate (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [gradlew*, gradle/**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README-native.md didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle.kts didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-native.yaml didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yml didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/Application.java didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/HelloController.java didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/springboot/HelloControllerTest.java didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug settings.gradle didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew matched [gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew.bat matched [gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.jar matched [gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug gradle/wrapper/gradle-wrapper.properties matched [gradlew*, gradle/**] -> included
┃ ┃ ┃ ┗ ┗ ┗ ┗ ╺ engine.transformations[1].validated.transformations[1].then.transformations[3].sources[1].validated.delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].apply (ReplaceText)
┃ ┃ ┃ ┗  Info Will replace [tanzu-java-web-app->my-web-app-axl]
┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[3].apply (ReplaceText)
┃ ┃ ┃ ┗  Info Will replace [tanzu-java-web-app->my-web-app-axl]
┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[4].apply (ReplaceText)
┃ ┃ ┃ ┗  Info Will replace [tanzu-java-web-app->my-web-app-axl]
┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[5].apply (ReplaceText)
┃ ┃ ┃ ┗  Info Will replace [tanzu-java-web-app->my-web-app-axl]
┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[6] (IfElse)
┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[6].then (Chain)
┃ ┃ ┃ ┃  Info Running Chain(ApplyTo, ApplyTo, RewritePath, UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[6].then.transformations[0].apply (ReplaceText)
┃ ┃ ┃ ┃ ┗  Info Will replace [tanzu-java-web-app->my-web-app-axl]
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[6].then.transformations[1].apply (ReplaceText)
┃ ┃ ┃ ┃ ┗  Info Will replace [tanzu-java-web-app->my-web-app-axl]
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[6].then.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┗ Debug Path 'README-native.md' matched 'README-native.md' with groups {g0=README-native.md} and was rewritten to 'README.md'
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[6].then.transformations[3] (UniquePath)
┃ ┃ ┃ ┗ ┗ Debug Multiple representations for path 'README.md', will concatenate them together
┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7] (Merge)
┃ ┃ ┃ ┃  Info Running Merge(Include, InvokeFragment, InvokeFragment, InvokeFragment)
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ Debug gradlew matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/springboot/HelloControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug settings.gradle matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.jar matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/HelloController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug gradlew.bat matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug build.gradle.kts matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug config/workload-native.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yml matched [**] -> included
┃ ┃ ┃ ┃ ┗ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Let
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate (Let)
┃ ┃ ┃ ┃ ┃ ┃ Debug Adding symbol workloadJavaVersion with value '21'
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[0].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[0].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/springboot/HelloControllerTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug settings.gradle didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.jar didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/HelloController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew.bat didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/Application.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle.kts didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-native.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[0].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '<java.version>.*<' with '<java.version>21<'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [build.gradle]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/springboot/HelloControllerTest.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug settings.gradle didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.jar didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/HelloController.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.properties didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew.bat didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/Application.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle.kts didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-native.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[1].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex 'sourceCompatibility = .*' with 'sourceCompatibility ...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[2].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[2].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [build.gradle.kts]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/springboot/HelloControllerTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug settings.gradle didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.jar didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/HelloController.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew.bat didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/Application.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle.kts matched [build.gradle.kts] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-native.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[2].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '(?<unmodified>JavaVersion\.VERSION_)(\d+)' with '${unmodified}21'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[3].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[3].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/workload.yaml, config/workload-native.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/springboot/HelloControllerTest.java didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug settings.gradle didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.jar didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/HelloController.java didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.properties didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew.bat didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/Application.java didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/workload.yaml, config/workload-native.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle.kts didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-native.yaml matched [config/workload.yaml, config/workload-native.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yml didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[3].delegate.transformations[1] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[4].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[4].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/*.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/springboot/HelloControllerTest.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug settings.gradle didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.jar didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/HelloController.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew.bat didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/springboot/Application.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/*.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle.kts didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-native.yaml matched [config/*.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[4].delegate.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [config/workload*.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/workload*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug config/workload-native.yaml matched [config/workload*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[0].sources[4].delegate.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace regex '(?<unmodified>image: bellsoft/liberica-openjdk-\w*:)(\d+)' with '${unmodified}21'
┃ ┃ ┃ ┃ ┗ ┗ ┗ ╺ engine.transformations[1].validated.transformations[7].sources[1].validated.delegate.in.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[2] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[2].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#includeDevContainer) evaluated to false
┃ ┃ ┃ ┃ ┗ ┗ null ()
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[3] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[3].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#bsGitRepository != null) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Let
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[7].sources[3].validated.delegate (Let)
┃ ┃ ┃ ┃ ┃ ┃ Debug Adding symbol repoUrl with value 'https://github.com?owner=trisberg&repo=my-web-app-axl'
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[3].validated.delegate.in.apply (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(OpenRewriteRecipe, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[1].validated.transformations[7].sources[3].validated.delegate.in.apply.transformations[0] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[7].sources[3].validated.delegate.in.apply.transformations[1] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗ ┗ ┗  Info Will replace regex '(?<beforeBranch>[\s\S]+)(?<branch>branch: [\S]+)(?<rest>[\S\s]*)' with '${beforeBranch}branc...(truncated)'
┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[8] (UniquePath)
┃ ┃ ┃ ┃ Debug Multiple representations for path 'src/test/java/com/example/springboot/HelloControllerTest.java', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'gradlew', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'settings.gradle', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path '.gitignore', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'gradle/wrapper/gradle-wrapper.jar', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'src/main/java/com/example/springboot/HelloController.java', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'gradle/wrapper/gradle-wrapper.properties', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'gradlew.bat', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'README.md', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'catalog/catalog-info.yaml', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'src/main/java/com/example/springboot/Application.java', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'build.gradle.kts', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'config/workload.yaml', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'Tiltfile', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'config/workload-native.yaml', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path '.tanzuignore', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'LICENSE', will use the one appearing last 
┃ ┃ ┃ ┗ Debug Multiple representations for path 'src/main/resources/application.yml', will use the one appearing last 
┃ ┗ ┗ ╺ engine.transformations[1].validated.transformations[9] (Provenance)
┗ ╺ engine.transformations[2] (UniquePath)
```
