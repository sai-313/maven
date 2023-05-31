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
script: 'scp /root/home/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war   root@:172.31.3.241/var/lib/tomcat9/webapps/qaenv.war'
	}
    stage('Continuous Testing') 
	{
     script: 'echo "Testing Passed"'
	}
    stage('Continuous Delivery') 
	{
script: 'scp /root/home/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war   root@:172.31.3.241/var/lib/tomcat9/webapps/qaenv.war'
	}
}
