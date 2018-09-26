node {
  stage('SCM checkout'){
    git 'https://github.com/abkharde/maven-pipeline'
  }
   stage('Compile package'){
     def mvnHome = tool name: 'maven-3.4', type: 'maven'
     dir('my-app') {
     sh "${mvnHome}/bin/mvn package"
     sh 'java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App'
	}
  }
  }
