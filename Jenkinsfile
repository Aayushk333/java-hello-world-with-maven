node{
  stage('SCM Checkout'){
    git 'https://github.com/Aayushk333/java-hello-world-with-maven'
  }
  stage('Compile-Package'){
    sh 'mvn package'
  }
}
