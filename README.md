# emfinfo.github.io
A generic repository for Java .jar libraries. 

Here is some documentation for the libraries :<br>
http://www.jcsinfo.ch/doc/basiclib<br>
http://www.jcsinfo.ch/doc/cypherlib<br>
http://www.jcsinfo.ch/doc/daolayer<br>
http://www.jcsinfo.ch/doc/playlib<br>
http://www.jcsinfo.ch/doc/javafxlib

To link a Maven project with a library here, you must add some lines in your pom.xml (build file). Example :

    <!-- additional repository -->  
    <repositories>
      <repository>
        <id>emfinfo</id>
        <name>emfinfo.github.io</name>
        <url>http://emfinfo.github.io/javalibs/releases</url>
      </repository>
    </repositories>      
    
    <!-- dependencies -->
    <dependencies>
      
      <!-- on BasicLib -->
      <dependency>       
        <groupId>ch.emf.info</groupId>
        <artifactId>basiclib</artifactId>
        <version>1.3.4</version>
      </dependency>
      
      <!-- on CypherLib  -->
      <dependency>       
        <groupId>ch.emf.info</groupId>
        <artifactId>cypherlib</artifactId>
        <version>1.1.0</version>
      </dependency>       
      
      <!-- on DaoLayer -->
      <dependency>       
        <groupId>ch.emf.info</groupId>
        <artifactId>daolayer</artifactId>
        <version>6.1.1</version>
      </dependency>   
      
      <!-- on PlayLib -->
      <dependency>       
        <groupId>ch.emf.info</groupId>
        <artifactId>playlib</artifactId>
        <version>1.1.0</version>
      </dependency>  
            
      <!-- on JavaFxLib -->
      <dependency>       
        <groupId>ch.emf.info</groupId>
        <artifactId>javafxlib</artifactId>
        <version>1.0.1</version>
      </dependency>      
      
    </dependencies>

For Scala SBT (Play! framework), add a resolver and necessary dependencies :<br>

    resolvers += "EMF-info Repository" at "http://emfinfo.github.io/javalibs/releases"
    
    libraryDependencies ++Seq= (
      "ch.emf.info" % "basiclib" % "1.3.4", 
      "ch.emf.info" % "cypherlib" % "1.1.0",
      "ch.emf.info" % "daolayer" % "6.1.1",
      "ch.emf.info" % "playlib" % "1.1.0",
      "ch.emf.info" % "javafxlib" % "1.0.1",
      ...
    )    
