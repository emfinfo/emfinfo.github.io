# emfinfo.github.io
A generic repository for Java .jar libraries of the EMF school. To link a Maven project with a library here, you must add some lines in your pom.xml (build file). Example :

    <!-- additional repository -->  
    <repositories>
      <repository>        
        <id>emfinfo</id>
        <name>emfinfo.github.io</name>
        <url>http://emfinfo.github.io/javalibs/releases</url>
      </repository>
      
    </repositories>      
    
    <dependencies>
      <!-- dependencies for BasicLib -->
      <dependency>       
        <groupId>ch.emf.info</groupId>
        <artifactId>basiclib</artifactId>
        <version>1.01</version>
      </dependency> 
      
      <!-- dependencies for DaoLayer -->
      <dependency>       
        <groupId>ch.emf.info</groupId>
        <artifactId>daolayer</artifactId>
        <version>5.34</version>
      </dependency>    
    </dependencies>

For Scala SBT (Play! framework), add a resolver and necessary dependencies :<br>

    resolvers += "EMF-info Repository" at "http://emfinfo.github.io/javalibs/releases"
    
    libraryDependencies ++Seq= (
      "ch.emf.info" % "basiclib" % "1.01",
      "ch.emf.info" % "daolayer" % "5.34",
      ...
    )    
