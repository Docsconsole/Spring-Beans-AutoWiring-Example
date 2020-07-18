# Spring-Beans-AutoWiring-Example
Spring-Beans-AutoWiring-Example


C:\USERS\D951857\WORKSPACE\SPRINGCOREWS\SPRING-BEANS-AUTOWIRING-EXAMPLE
|   pom.xml
|   Spring-Beans-AutoWiring-Example.iml
|
+---.idea
|       .gitignore
|       compiler.xml
|       jarRepositories.xml
|       misc.xml
|       uiDesigner.xml
|       workspace.xml
|
+---src
|   +---main
|   |   +---java
|   |   |   \---com
|   |   |       \---docsconsole
|   |   |           \---spring5
|   |   |               \---autowiring
|   |   |                   +---annotations
|   |   |                   |   +---onproperties
|   |   |                   |   |       AppConfig.java
|   |   |                   |   |       ASpringBean.java
|   |   |                   |   |       BSpringBean.java
|   |   |                   |   |       MainAppClient.java
|   |   |                   |   |
|   |   |                   |   +---onsetter
|   |   |                   |   |       AppConfig.java
|   |   |                   |   |       ASpringBean.java
|   |   |                   |   |       BSpringBean.java
|   |   |                   |   |       MainAppClient.java
|   |   |                   |   |
|   |   |                   |   \---qualifier
|   |   |                   |       +---autowiringproblem
|   |   |                   |       |       AppConfig.java
|   |   |                   |       |       ASpringBean.java
|   |   |                   |       |       BSpringBean.java
|   |   |                   |       |       CSpringBean.java
|   |   |                   |       |       MainAppClient.java
|   |   |                   |       |       SpringBean.java
|   |   |                   |       |
|   |   |                   |       \---autowiringsolution
|   |   |                   |               AppConfig.java
|   |   |                   |               ASpringBean.java
|   |   |                   |               BSpringBean.java
|   |   |                   |               CSpringBean.java
|   |   |                   |               MainAppClient.java
|   |   |                   |               SpringBean.java
|   |   |                   |
|   |   |                   \---xml
|   |   |                       +---onconstructor
|   |   |                       |       ASpringBean.java
|   |   |                       |       BSpringBean.java
|   |   |                       |       MainAppClient.java
|   |   |                       |
|   |   |                       +---onproperties
|   |   |                       |       ASpringBean.java
|   |   |                       |       BSpringBean.java
|   |   |                       |       MainAppClient.java
|   |   |                       |
|   |   |                       \---onsetter
|   |   |                               ASpringBean.java
|   |   |                               BSpringBean.java
|   |   |                               MainAppClient.java
|   |   |
|   |   \---resources
|   |           spring-beans.xml
|   |           spring-beans1.xml
|   |           spring-beans2.xml
|   |
|   \---test
|       \---java
\---target
    |   Spring-Beans-AutoWiring-Example-1.0-SNAPSHOT.jar
    |
    +---classes
    |   |   spring-beans.xml
    |   |   spring-beans1.xml
    |   |   spring-beans2.xml
    |   |
    |   +---com
    |   |   \---docsconsole
    |   |       \---spring5
    |   |           \---autowiring
    |   |               +---annotations
    |   |               |   +---onproperties
    |   |               |   |       AppConfig.class
    |   |               |   |       ASpringBean.class
    |   |               |   |       BSpringBean.class
    |   |               |   |       MainAppClient.class
    |   |               |   |
    |   |               |   +---onsetter
    |   |               |   |       AppConfig.class
    |   |               |   |       ASpringBean.class
    |   |               |   |       BSpringBean.class
    |   |               |   |       MainAppClient.class
    |   |               |   |
    |   |               |   \---qualifier
    |   |               |       +---autowiringproblem
    |   |               |       |       AppConfig.class
    |   |               |       |       ASpringBean.class
    |   |               |       |       BSpringBean.class
    |   |               |       |       CSpringBean.class
    |   |               |       |       MainAppClient.class
    |   |               |       |       SpringBean.class
    |   |               |       |
    |   |               |       \---autowiringsolution
    |   |               |               AppConfig.class
    |   |               |               ASpringBean.class
    |   |               |               BSpringBean.class
    |   |               |               CSpringBean.class
    |   |               |               MainAppClient.class
    |   |               |               SpringBean.class
    |   |               |
    |   |               \---xml
    |   |                   +---onconstructor
    |   |                   |       ASpringBean.class
    |   |                   |       BSpringBean.class
    |   |                   |       MainAppClient.class
    |   |                   |
    |   |                   +---onproperties
    |   |                   |       ASpringBean.class
    |   |                   |       BSpringBean.class
    |   |                   |       MainAppClient.class
    |   |                   |
    |   |                   \---onsetter
    |   |                           ASpringBean.class
    |   |                           BSpringBean.class
    |   |                           MainAppClient.class
    |   |
    |   \---META-INF
    |           Spring-Beans-AutoWiring-Example.kotlin_module
    |
    +---generated-sources
    |   \---annotations
    +---maven-archiver
    |       pom.properties
    |
    \---maven-status
        \---maven-compiler-plugin
            +---compile
            |   \---default-compile
            |           createdFiles.lst
            |           inputFiles.lst
            |
            \---testCompile
                \---default-testCompile
                        inputFiles.lst
                        
                        
                        
                        
                        
