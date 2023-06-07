pipeline {
    agent any

    stages {
        stage('Git Tagging') {
            steps {
                script {
                    def tagName = "v1.8" // Set your desired tag name here

                    sh "git tag ${tagName}" // Creates the Git tag
                    sh "git push origin ${tagName}" // Pushes the tag to the remote repository
                }
            }
        }
        // Other stages in your pipeline...
    }
}
