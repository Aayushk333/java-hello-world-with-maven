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
    
    sh "java -jar /Users/Shared/Jenkins/Home/workspace/jenkinsfile-git-and-maven/target/jb-hello-world-maven-0.1.0-shaded.jar"
    
    
  }
}
