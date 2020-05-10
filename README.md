# emfinfo.github.io
A generic repository for Java .jar libraries. 

Here is some documentation for the libraries :<br>
https://www.jcsinfo.ch/doc/basiclib<br>
https://www.jcsinfo.ch/doc/cypherlib<br>
https://www.jcsinfo.ch/doc/daolayer<br>
https://www.jcsinfo.ch/doc/playlib<br>
https://www.jcsinfo.ch/doc/javafxlib

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
        <groupId>ch.jdsinfo.libs</groupId>
        <artifactId>basiclib</artifactId>
        <version>1.5.0</version>
      </dependency>
      
      <!-- on CypherLib  -->
      <dependency>       
        <groupId>ch.jcsinfo.libs</groupId>
        <artifactId>cypherlib</artifactId>
        <version>1.2.1</version>
      </dependency>       
      
      <!-- on PlayLib -->
      <dependency>       
        <groupId>ch.jcsinfo.libs</groupId>
        <artifactId>playlib</artifactId>
        <version>2.8.1</version>
      </dependency>  
            
      <!-- on JavaFxLib -->
      <dependency>       
        <groupId>ch.jcsinfo.libs</groupId>
        <artifactId>javafxlib</artifactId>
        <version>8.0.1</version>
      </dependency>      

      <!-- on DaoLayer -->
      <dependency>       
        <groupId>ch.emf.info</groupId>
        <artifactId>daolayer</artifactId>
        <version>6.1.1</version>
      </dependency>   
            
    </dependencies>

For Scala SBT (Play! framework), add a resolver and necessary dependencies :<br>

    resolvers += "EMF-info Repository" at "http://emfinfo.github.io/javalibs/releases"
    
    libraryDependencies ++Seq= (
      "ch.jcsinfo.libs" % "basiclib" % "1.5.0", 
      "ch.jcsinfo.libs" % "cypherlib" % "1.2.1",
      "ch.jcsinfo.libs" % "playlib" % "2.8.1",
      "ch.jcsinfo.libs" % "javafxlib" % "8.0.1",
      "ch.emf.info" % "daolayer" % "6.1.1"
      ...
    )    
