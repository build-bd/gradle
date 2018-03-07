### Gradle to use Specific JDK
#### 1. Gradle Command Line argument
```sh
gradle build -Dorg.gradle.java.home=/opt/jdk
gradle build -Dorg.gradle.java.home=/opt/openjdk
```

#### 2. Gradle Properties File
##### i. Global Way
* In ``` gradle.properties ``` in the ``` .gradle ``` directory in your 
* ``` HOME_DIRECTORY [~/.gradle/] ``` set ``` org.gradle.java.home=/opt/jdk ```
* ``` HOME_DIRECTORY [~/.gradle/] ``` set ``` org.gradle.java.home=/opt/openjdk ```
##### ii. Project Specific
* ``` gradle.properties ``` can be used in project level means in project root directory

#### 3. Temporary ` JAVA_HOME ` Environment Variable
* Open Command Prompt ` cmd `
* Run Following Command ` set JAVA_HOME="D:\tools\jdk\ojdk10" `
* Test Successful ` JAVA_HOME ` setup using ` echo %JAVA_HOME% `
* Now Build Gradle using ` gradle build ` command
* See From Task Manager which Java is using gradle to build the project
