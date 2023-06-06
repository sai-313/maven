pipeline {
  agent any

  stages {
    stage('Git Checkout') {
      steps {
        git branch: 'master', url: 'https://github.com/sai-313/maven.git'
      }
    }

    stage('Build') {
      // Your build steps
    }

    stage('Tagging') {
      steps {
        script {
          def tag = "v1.0" // Define the tag name you want to create
          sh "git tag ${tag}"
          sh "git push origin ${tag}"
        }
      }
    }

    stage('Test') {
      // Your testing steps
    }

    stage('Deploy') {
      // Your deployment steps
    }
  }
}
