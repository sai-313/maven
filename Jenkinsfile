node('built-in') 
{
    stage('Continuous Download') 
	{
    git 'https://github.com/sai-313/hello-world-war.git'
	}
    stage('Continuous Build') 
	{
    script: 'mvn package'
	}
}
