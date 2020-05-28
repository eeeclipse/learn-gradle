# learn-gradle ! 


Gradle is an open-source, general-purpose build tool. It is popular in the Java community and is the preferred build tool for Android.


# Requirements
- [Java JDK or JRE (version 7 or higher for Gradle 3.x version](https://www.oracle.com/java/technologies/javase-downloads.html)

# Installation

## Install gradle on mac

```Shell
$ brew install gradle
```

```Shell
$ gradle --version
```

## Install gradle on Windows

1. Download Gradle distribution from the official web site
2. Unpack the ZIP
3. Add the GRADLE_HOME environment variable. This variable should point to the unpacked files from the previous step.
4. Add GRADLE_HOME/bin to your PATH environment variable, so you can run Gradle from the command line interface (CLI)
Test your Gradle installation by typing gradle -v in the CLI. The output should contain the installed Gradle version and the current Gradle configuration details

# Hello World

Let's make a simple gradle project. Gradle tasks can be written using Groovy code from inside a projects build.gradle file. These tasks can then be executed using ```> gradle [taskname]``` at the terminal or by executing the task from within an IDE such as Eclipse. To create the Hello World example in gradle we must define a task that will print a string to the console using Groovy. We will use Groovy's ```printLn``` to call Java's ```System.out.printLn``` method to print the text to the console.

```javascript
##build.gradle
task hello {
    doLast {
        println 'Hello world!'
    }
}
```


 


# Reference 
- [Maven을 넘어 Gradle로 가자.](http://kwon37xi.egloos.com/4747016)
- [slipp.net/wiki](https://www.slipp.net/wiki/display/IDE/Gradle)
- [Gradle Basic - How to use Gradle in Java Project](https://www.slideshare.net/ienvyou/gradle-basic-how-to-use-gradle-in-java-project)
