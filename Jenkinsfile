node('built-in') 
{
    stage('Continuous Download') 
	{
    git 'https://github.com/sai-313/maven.git'
	}
    stage('Continuous Build') 
	{
    script: 'mvn package'
	}
	stage('Tagging') {
            steps {
                script {
                    def gitTag = "v1.5" // Specify the tag name here
                    sh "git tag ${gitTag}"
                    sh "git push origin ${gitTag}"
                }
            }
        }
}
