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
