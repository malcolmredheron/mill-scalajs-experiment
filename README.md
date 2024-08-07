
Repro steps:
- `git clean -xdf` just to be sure
- `./mill mill.idea.GenIdea/idea + app.compile`
- Open the project in IntelliJ, such as with `idea-ultimate . >/dev/null 2>&1 &`

Building on the command line works, but building in IntelliJ (control-F9) fails with the following error for any version of Scala 3 that I have tried (set in build.sc):

`scala: Multiple 'scala3-library*.jar' files (scala3-library_3-3.3.1.jar, scala3-library_sjs1_3-3.3.1.jar) in Scala compiler classpath in Scala SDK scala-SDK-3.3.1`