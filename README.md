maven-repo
==========

This is a temporary Maven repository. You publish to it from projects by adding the following line to sbt:

  publishTo := Some(Resolver.file("file",  new File("../maven-repo/releases")))
    
To consume the repo, the github url has to be listed in the resolvers:


  "VictorOps Repository" at "https://raw.github.com/fooblahblah/maven-repo/master/releases"
  
