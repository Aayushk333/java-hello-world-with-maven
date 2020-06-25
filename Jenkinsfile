node{
  stage('SCM Checkout'){
    git 'https://github.com/Aayushk333/java-hello-world-with-maven'
  }
  stage('Compile-Package'){
    // Get Maven Home Path
    def mvnHome = tool name: 'apache-maven-3.6.3', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
  
  stage('Build'){
    echo 'Build starting ! ...'
    sh "pwd"
    sh "cd src/main/java/hello"
    sh "java HelloWorld.java"
    
    
    
  }
}
