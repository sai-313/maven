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
}
