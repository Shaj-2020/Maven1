node('master')
{ 
stage('continuousdownload_loans')
{
git 'https://github.com/Shaj-2020/Maven1.git'
}
stage('continuousBuild_loans')
{
sh label: '', script: 'mvn package'
}
stage('ContinuousDeployment_loans')
{
sh label: '', script: 'scp /root/.jenkins/workspace/ScriptedPipeline/memoryref/target/memoryref.jar ec2-user@54.89.207.243:/var/lib/tomcat/webapps/qaapp.jar'
}
}
