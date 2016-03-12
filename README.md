# emfinfo.github.io
A generic repository for Java .jar libraries of the EMF school. To use this library in a Maven project, you can add some  lines in your pom.xml. See the wiki for an example.

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
      <dependency>       
        <groupId>ch.jcsinfo</groupId>
        <artifactId>basiclib</artifactId>
        <version>1.xx</version>
      </dependency>    
    </dependencies>
