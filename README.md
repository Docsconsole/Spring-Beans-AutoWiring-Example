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
                        
                        
                        



package com.docsconsole.spring5.autowiring.annotations.onproperties;

import org.springframework.context.annotation.ComponentScan;
import org.springframework.context.annotation.Configuration;

@Configuration
@ComponentScan(basePackages = "com.docsconsole.spring5.autowiring.annotations.onproperties")
public class AppConfig {


}




package com.docsconsole.spring5.autowiring.annotations.onproperties;

import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Component;

@Component("aSpringBean")
public class ASpringBean {

    @Autowired
    private BSpringBean bSpringBean;

    public BSpringBean getbSpringBean() {
        return bSpringBean;
    }


    public void setbSpringBean(BSpringBean bSpringBean) {
        this.bSpringBean = bSpringBean;
    }
    public void getBStringBeanName(){
        bSpringBean.getBSpringBeanName();
    }
}





package com.docsconsole.spring5.autowiring.annotations.onproperties;

import org.springframework.stereotype.Component;

@Component("bSpringBean")
public class BSpringBean {

    public BSpringBean() {
        System.out.println("Testing Auto-wiring Concept.");
    }
    public void getBSpringBeanName(){
        System.out.println("The BSpringBeanName ");
    }
}





package com.docsconsole.spring5.autowiring.annotations.onproperties;

import org.springframework.context.annotation.AnnotationConfigApplicationContext;

public class MainAppClient {
    public static void main(String[] args) {

        AnnotationConfigApplicationContext context = new AnnotationConfigApplicationContext(AppConfig.class);
        ASpringBean aSpringBean = context.getBean(ASpringBean.class);
        aSpringBean.getbSpringBean().getBSpringBeanName();
        context.close();

    }
}






package com.docsconsole.spring5.autowiring.annotations.onsetter;

import org.springframework.context.annotation.ComponentScan;
import org.springframework.context.annotation.Configuration;

@Configuration
@ComponentScan(basePackages = "com.docsconsole.spring5.autowiring.annotations.onsetter")
public class AppConfig {


}





package com.docsconsole.spring5.autowiring.annotations.onsetter;

import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Component;

@Component("aSpringBean")
public class ASpringBean {

    private BSpringBean bSpringBean;

    public BSpringBean getbSpringBean() {
        return bSpringBean;
    }

    @Autowired
    public void setbSpringBean(BSpringBean bSpringBean) {
        this.bSpringBean = bSpringBean;
    }
    public void getBStringBeanName(){
        bSpringBean.getBSpringBeanName();
    }
}



package com.docsconsole.spring5.autowiring.annotations.onsetter;

import org.springframework.stereotype.Component;

@Component("bSpringBean")
public class BSpringBean {

    public BSpringBean() {
        System.out.println("Testing Auto-wiring Concept.");
    }
    public void getBSpringBeanName(){
        System.out.println("The BSpringBeanName ");
    }
}



package com.docsconsole.spring5.autowiring.annotations.onsetter;

import org.springframework.context.annotation.AnnotationConfigApplicationContext;

public class MainAppClient {
    public static void main(String[] args) {

        AnnotationConfigApplicationContext context = new AnnotationConfigApplicationContext(AppConfig.class);
        ASpringBean aSpringBean = context.getBean(ASpringBean.class);
        aSpringBean.getbSpringBean().getBSpringBeanName();
        context.close();

    }
}



package com.docsconsole.spring5.autowiring.annotations.qualifier.autowiringproblem;

import org.springframework.context.annotation.ComponentScan;
import org.springframework.context.annotation.Configuration;

@Configuration
@ComponentScan(basePackages = "com.docsconsole.spring5.autowiring.annotations.qualifier.autowiringproblem")
public class AppConfig {


}






package com.docsconsole.spring5.autowiring.annotations.qualifier.autowiringproblem;


import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Component;

@Component("aSpringBean")
public class ASpringBean {

    @Autowired
    private SpringBean springBean;

    public SpringBean getSpringBean() {
        return springBean;
    }

    public void setSpringBean(SpringBean springBean) {
        this.springBean = springBean;
    }

    public void getSpringBeanName(){
        springBean.getSpringBeanName();
    }
}





package com.docsconsole.spring5.autowiring.annotations.qualifier.autowiringproblem;

import org.springframework.stereotype.Component;

@Component("bSpringBean")
public class BSpringBean implements SpringBean {

    public BSpringBean() {
        System.out.println("Testing Auto-wiring Concept.");
    }
    public void getSpringBeanName(){
        System.out.println("The BSpringBeanName ");
    }
}




package com.docsconsole.spring5.autowiring.annotations.qualifier.autowiringproblem;

import org.springframework.stereotype.Component;

@Component("CSpringBean")
public class CSpringBean implements SpringBean {

    public CSpringBean() {
        System.out.println("Testing Auto-wiring Concept.");
    }
    public void getSpringBeanName(){
        System.out.println("The CSpringBeanName ");
    }
}





package com.docsconsole.spring5.autowiring.annotations.qualifier.autowiringproblem;

import org.springframework.context.annotation.AnnotationConfigApplicationContext;

public class MainAppClient {
    public static void main(String[] args) {

        AnnotationConfigApplicationContext context = new AnnotationConfigApplicationContext(AppConfig.class);
        ASpringBean aSpringBean = context.getBean(ASpringBean.class);
        aSpringBean.getSpringBeanName();
        context.close();

    }
}





package com.docsconsole.spring5.autowiring.annotations.qualifier.autowiringproblem;

public interface SpringBean {
    public void getSpringBeanName();
}






package com.docsconsole.spring5.autowiring.annotations.qualifier.autowiringsolution;

import org.springframework.context.annotation.ComponentScan;
import org.springframework.context.annotation.Configuration;

@Configuration
@ComponentScan(basePackages = "com.docsconsole.spring5.autowiring.annotations.qualifier.autowiringsolution")
public class AppConfig {


}






package com.docsconsole.spring5.autowiring.annotations.qualifier.autowiringsolution;


import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.beans.factory.annotation.Qualifier;
import org.springframework.stereotype.Component;

@Component("aSpringBean")
public class ASpringBean {

    @Autowired
    @Qualifier("bSpringBean")
    private SpringBean springBean;

    public SpringBean getSpringBean() {
        return springBean;
    }

    public void setSpringBean(SpringBean springBean) {
        this.springBean = springBean;
    }

    public void getSpringBeanName(){
        springBean.getSpringBeanName();
    }
}





package com.docsconsole.spring5.autowiring.annotations.qualifier.autowiringsolution;

import org.springframework.stereotype.Component;

@Component("bSpringBean")
public class BSpringBean implements SpringBean {

    public BSpringBean() {
        System.out.println("Testing Auto-wiring Concept.");
    }
    public void getSpringBeanName(){
        System.out.println("The BSpringBeanName ");
    }
}








package com.docsconsole.spring5.autowiring.annotations.qualifier.autowiringsolution;

import org.springframework.stereotype.Component;

@Component("CSpringBean")
public class CSpringBean implements SpringBean {

    public CSpringBean() {
        System.out.println("Testing Auto-wiring Concept.");
    }
    public void getSpringBeanName(){
        System.out.println("The CSpringBeanName ");
    }
}







package com.docsconsole.spring5.autowiring.annotations.qualifier.autowiringsolution;

import org.springframework.context.annotation.AnnotationConfigApplicationContext;

public class MainAppClient {
    public static void main(String[] args) {

        AnnotationConfigApplicationContext context = new AnnotationConfigApplicationContext(AppConfig.class);
        ASpringBean aSpringBean = context.getBean(ASpringBean.class);
        aSpringBean.getSpringBeanName();
        context.close();

    }
}





package com.docsconsole.spring5.autowiring.annotations.qualifier.autowiringsolution;

public interface SpringBean {
    public void getSpringBeanName();
}




package com.docsconsole.spring5.autowiring.xml.onconstructor;

import org.springframework.beans.factory.annotation.Autowired;

public class ASpringBean {

    private BSpringBean bSpringBean;

    @Autowired
    public ASpringBean(BSpringBean bSpringBean){
        this.bSpringBean = bSpringBean;
    }



    public BSpringBean getbSpringBean() {
        return bSpringBean;
    }

    public void setbSpringBean(BSpringBean bSpringBean) {
        this.bSpringBean = bSpringBean;
    }
    public void getBStringBeanName(){
        bSpringBean.getBSpringBeanName();
    }
}







package com.docsconsole.spring5.autowiring.xml.onconstructor;

public class BSpringBean {

    public BSpringBean() {
        System.out.println("Testing Auto-wiring Concept.");
    }
    public void getBSpringBeanName(){
        System.out.println("The BSpringBeanName ");
    }
}






package com.docsconsole.spring5.autowiring.xml.onconstructor;

import org.springframework.context.ConfigurableApplicationContext;
import org.springframework.context.support.ClassPathXmlApplicationContext;

public class MainAppClient {
    public static void main(String[] args) {

        ConfigurableApplicationContext context = new ClassPathXmlApplicationContext("spring-beans2.xml");
        ASpringBean aSpringBean = (ASpringBean) context.getBean("aSpringBean");
        aSpringBean.getbSpringBean().getBSpringBeanName();
        context.close();

    }
}






package com.docsconsole.spring5.autowiring.xml.onproperties;

import org.springframework.beans.factory.annotation.Autowired;

public class ASpringBean {

    @Autowired
    private BSpringBean bSpringBean;

    public BSpringBean getbSpringBean() {
        return bSpringBean;
    }


    public void setbSpringBean(BSpringBean bSpringBean) {
        this.bSpringBean = bSpringBean;
    }
    public void getBStringBeanName(){
        bSpringBean.getBSpringBeanName();
    }
}





package com.docsconsole.spring5.autowiring.xml.onproperties;

public class BSpringBean {

    public BSpringBean() {
        System.out.println("Testing Auto-wiring Concept.");
    }
    public void getBSpringBeanName(){
        System.out.println("The BSpringBeanName ");
    }
}






package com.docsconsole.spring5.autowiring.xml.onproperties;

import org.springframework.context.ConfigurableApplicationContext;
import org.springframework.context.support.ClassPathXmlApplicationContext;

public class MainAppClient {
    public static void main(String[] args) {

        ConfigurableApplicationContext context = new ClassPathXmlApplicationContext("spring-beans1.xml");
        ASpringBean aSpringBean = (ASpringBean) context.getBean("aSpringBean");
        aSpringBean.getbSpringBean().getBSpringBeanName();
        context.close();

    }
}







package com.docsconsole.spring5.autowiring.xml.onsetter;

import org.springframework.beans.factory.annotation.Autowired;

public class ASpringBean {

    private BSpringBean bSpringBean;

    public BSpringBean getbSpringBean() {
        return bSpringBean;
    }

    @Autowired
    public void setbSpringBean(BSpringBean bSpringBean) {
        this.bSpringBean = bSpringBean;
    }
    public void getBStringBeanName(){
        bSpringBean.getBSpringBeanName();
    }
}






package com.docsconsole.spring5.autowiring.xml.onsetter;

public class BSpringBean {

    public BSpringBean() {
        System.out.println("Testing Auto-wiring Concept.");
    }
    public void getBSpringBeanName(){
        System.out.println("The BSpringBeanName ");
    }
}






package com.docsconsole.spring5.autowiring.xml.onsetter;

import org.springframework.context.ConfigurableApplicationContext;
import org.springframework.context.support.ClassPathXmlApplicationContext;

public class MainAppClient {
    public static void main(String[] args) {

        ConfigurableApplicationContext context = new ClassPathXmlApplicationContext("spring-beans.xml");
        ASpringBean aSpringBean = (ASpringBean) context.getBean("aSpringBean");
        aSpringBean.getbSpringBean().getBSpringBeanName();
        context.close();

    }
}








<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xmlns:context="http://www.springframework.org/schema/context"
       xmlns="http://www.springframework.org/schema/beans"
       xsi:schemaLocation="http://www.springframework.org/schema/beans
   http://www.springframework.org/schema/beans/spring-beans.xsd
   http://www.springframework.org/schema/context
   http://www.springframework.org/schema/context/spring-context.xsd">

    <context:annotation-config/>

    <bean id="aSpringBean" class="com.docsconsole.spring5.autowiring.xml.onsetter.ASpringBean">
    </bean>
    <bean id="bSpringBean" class="com.docsconsole.spring5.autowiring.xml.onsetter.BSpringBean">
    </bean>
</beans>





<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xmlns:context="http://www.springframework.org/schema/context"
       xmlns="http://www.springframework.org/schema/beans"
       xsi:schemaLocation="http://www.springframework.org/schema/beans
   http://www.springframework.org/schema/beans/spring-beans.xsd
   http://www.springframework.org/schema/context
   http://www.springframework.org/schema/context/spring-context.xsd">

    <context:annotation-config/>

    <bean id="aSpringBean" class="com.docsconsole.spring5.autowiring.xml.onproperties.ASpringBean">
    </bean>
    <bean id="bSpringBean" class="com.docsconsole.spring5.autowiring.xml.onproperties.BSpringBean">
    </bean>
</beans>









<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xmlns:context="http://www.springframework.org/schema/context"
       xmlns="http://www.springframework.org/schema/beans"
       xsi:schemaLocation="http://www.springframework.org/schema/beans
   http://www.springframework.org/schema/beans/spring-beans.xsd
   http://www.springframework.org/schema/context
   http://www.springframework.org/schema/context/spring-context.xsd">

    <context:annotation-config/>

    <bean id="aSpringBean" class="com.docsconsole.spring5.autowiring.xml.onconstructor.ASpringBean">
    </bean>
    <bean id="bSpringBean" class="com.docsconsole.spring5.autowiring.xml.onconstructor.BSpringBean">
    </bean>
</beans>





                        
