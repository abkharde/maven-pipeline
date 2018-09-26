node {
  stage('SCM checkout'){
    git 'https://github.com/abkharde/maven-pipeline'
  }
   stage('Compile package'){
     def mvnHome = tool name: 'maven-3.4', type: 'maven'
     dir('my-app') {
      some block
     sh "${mvnHome}/bin/mvn package"
	}
  }
}
