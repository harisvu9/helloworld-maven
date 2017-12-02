node {
  stage('checkout'){
    checkout scm
  }

  stage('build'){
    dir('${WORKSPACE}/my-app'){
      sh 'mvn clean install'
    }
  }
  stage('sonar'){
    dir('${WORKSPACE}/my-app'){
      sh 'mvn sonar:sonar
    }
  }
  stage('package'){
    sh 'echo "Jenkinsfile"'
  }
  stage('deploy'){
    sh 'echo "Jenkinsfile"'
  }
}
