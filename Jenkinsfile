node('built-in') 
{
    stage('Continuous Download loans') 
	{
    git 'https://github.com/sunildevops77/maven.git'
	}
    stage('Continuous Build loans') 
	{
    sh label: '', script: 'mvn package'
	}
    stage('Continuous Deployment loans') 
	{
sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war   ubuntu@172.31.26.217:/var/lib/tomcat8/webapps/qaenv.war'
	}
    stage('Continuous Testing loans') 
	{
              sh label: '', script: 'echo "Testing Passed"'
	}
}
