# emfinfo.github.io
A generic repository for Java .jar libraries of the EMF school. To use this library in a Maven project, you can add this lines in your pom.xml :

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
      <version>1.01</version>
    </dependency>    
  </dependencies>
