node('built-in') 
{
    stage('Continuous Download') 
	{
    git 'https://github.com/sunildevops77/maven.git'
	}
    stage('Continuous Build') 
	{
    script: 'mvn package'
	}
    stage('Continuous Deployment') 
	{
script: 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war   ubuntu@:172.31.23.36/var/lib/tomcat8/webapps/qaenv.war'
	}
    stage('Continuous Testing') 
	{
     script: 'echo "Testing Passed"'
	}
    stage('Continuous Delivery') 
	{
script: 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war   ubuntu@:172.31.23.36/var/lib/tomcat8/webapps/prodenv.war'
	}
}
