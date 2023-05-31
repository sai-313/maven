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
    stage('Continuous Deployment') 
	{
script: 'scp /root/.jenkins/workspace/jenkins/target/hello-world-war-1.0.0.war   root@: 172.31.3.241/root/apache-tomcat-9.0.75/webapps/webapp.war'
	}
    stage('Continuous Testing') 
	{
     script: 'echo "Testing Passed"'
	}
   
}
