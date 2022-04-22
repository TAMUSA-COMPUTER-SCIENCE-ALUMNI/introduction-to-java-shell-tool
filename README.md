# Introduction to the Java Shell (JShell) Tool
The Java Shell tool (JShell) is an interactive tool for learning the Java programming language and prototyping Java code. JShell is a Read-Evaluate-Print Loop (REPL), which evaluates declarations, statements, and expressions as they are entered and immediately shows the results. The tool is run from the command line.

## Instructions
1. Check your the Java version installed on your machine via your cmd tool, powershell, or terminal console: 
```
    $ java -version
```
* You must have JDK 9 or higher installed
2. Open JShell: 
```
    $ jshell
```
3. Exit JShell:
```
    > /exit
```
4. Open JShell in verbose mode:
```
    $ jshell -v
```
5. Watch the [video]()

Oracle JDK 11 [JShell Documentation](https://docs.oracle.com/en/java/javase/11/jshell/introduction-jshell.html)


## JShell Commands
* To list all the declared variables.
```
    > /vars
    > /vars <variableName>
    > /vars <variableSnippetId>
    > /vars -start
    > /vars -all
```
*Example:*
```
    jshell> /vars
    |       String name = "OneCompiler"
    |       int id = 1
```
* To list all the declared Methods
```
    > /methods
    > /methods <methodName>
    > /methods <methodSnippetId>
    > /methods -start
    > /methods -all
```
*Example:*
```
    jshell> /methods
    |    double sum(int,int)
```
* To displays classes, interfaces, and enums
```
    > /types
    > /types <typeName>
    > /types <typeSnippetId>
    > /types -start
    > /types -all
```
* To see a list all the snippets
```
    > /list
    > /list -all
    > /list -start
    > /list <snippetName>
    > /list <snippetId>
```
* To save your snippets
```
    > /save
```
* To personalize your startup entries
```
    > /set start
```
* To get help about the list of the JShell commands.
```
    > /help
```
* To edit code of a method
```
    > /edit method-name
```
* To load Code from External Java File into REPL:
```
    > /open filename.java
```
* You can also provide directory information along wwith filename.java if the file is present in different directory like:
```
    > /open c:\\Documents\\filename.java
```
* To Drop a Snippet
```
    > /drop <snippetName>
    > /drop <snippetId> 
```
