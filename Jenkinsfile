node {
  stage('checkout'){
    checkout scm
  }

  stage('build'){
    dir('my-app'){
      sh 'mvn clean install sonar:sonar'
    }
  }
  // stage('sonar'){
  //   dir('my-app'){
  //     sh 'mvn sonar:sonar'
  //   }
  // }
  //stage('package'){
  //  sh 'echo "Jenkinsfile"'
  //}
  stage('deploy'){
    dir('my-app'){
    sh 'java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App'
  }
}
