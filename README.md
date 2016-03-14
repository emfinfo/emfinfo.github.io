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
    
    <!-- dependencies for BasicLib -->
    <dependencies>
      <dependency>       
        <groupId>ch.jcsinfo</groupId>
        <artifactId>basiclib</artifactId>
        <version>1.01</version>
      </dependency>    
    </dependencies>

    <!-- dependencies for DaoLayer -->
    <dependencies>
      <dependency>       
        <groupId>ch.emfinfo</groupId>
        <artifactId>daolayer</artifactId>
        <version>5.34</version>
      </dependency>    
    </dependencies>
    
    Scala SBT for BasicLib :
      libraryDependencies += "ch.jcsinfo" % "basiclib" % "1.01"

    Scala SBT for DaoLayer :
      libraryDependencies += "ch.emfinfo" % "daolayer" % "5.34"
