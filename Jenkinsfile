node {
  stage('checkout'){
    checkout scm
  }

  stage('build'){
    dir('my-app'){
      sh 'mvn clean install'
    }
  }
  stage('sonar'){
    dir('my-app'){
      sh 'mvn sonar:sonar'
    }
  }
  stage('package'){
    sh 'echo "Jenkinsfile"'
  }
  stage('deploy'){
    sh 'echo "Jenkinsfile"'
  }
}
