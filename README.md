sa-java-gradle
==============

[![Build Status](https://travis-ci.org/softasap/sa-java-gradle.svg?branch=master)](https://travis-ci.org/softasap/sa-java-gradle)

Example of usage (all parameters are optional)

Simple


```YAML
  roles:
    - {
        role: "sa-java-gradle"
      }
```

Advanced:

```YAML

  roles:
    - {
        role: "sa-java-gradle",
        gradle_version: "3.3",
        gradle_install_dir: "/opt/gradle",
        option_gradle_in_path: false
      }

```      

Important!

For consistency of historic builds it is recommended to use gradlew wrapper.
How to deal with it?


Create a Gradle Wrapper:

a) Declares a wrapper task.

```java
build.gradle
task wrapper(type: Wrapper) {
    gradleVersion = '2.10' //we want gradle 2.10 to run this project
}
```

b) Run the wrapper task with gradle wrapper

```
$ gradle wrapper

:wrapper

BUILD SUCCESSFUL
1.3 The following files will be created, remember to add these files and folders to your version control system (e.g GitHub or Bitbucket).

|-gradle
  |--- wrapper
      |--- gradle-wrapper.jar
      |--- gradle-wrapper.properties
|-gradlew
|-gradlew.bat 
```

Review the gradlew file, a unix shell script to run the Gradle task


Copyright and license
---------------------

Code licensed under the [BSD 3 clause] (https://opensource.org/licenses/BSD-3-Clause) or the [MIT License] (http://opensource.org/licenses/MIT).

Subscribe for roles updates at [FB] (https://www.facebook.com/SoftAsap/)
