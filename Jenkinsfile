node {
  stage('SCM checkout'){
    git 'https://github.com/abkharde/maven-pipeline'
  }
   stage('Compile package'){
    sh 'mvn package'
  }
}
