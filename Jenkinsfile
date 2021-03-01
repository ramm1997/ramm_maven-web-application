node
{
def mavenHome = tool name: "maven3.6.3" 

stage('CheckoutCode')
{
git branch: 'development', url: 'https://github.com/BagepalliAravindreddy/maven-web-application.git'
}

stage('BuildCode')
{
sh "${mavenHome}/bin/mvn clean package"
}
/*
stage('ExecuteSonarQubeReport')
{
sh "${mavenHome}/bin/mvn sonar:sonar"
}

stage('UploadArtifactIntoNexus')
{
sh "${mavenHome}/bin/mvn deploy"
}
stage('DeployAppIntoTomcatServer')
{
sshagent(['53b047e0-3b85-4112-93d1-78560ff89b48']) {
sh "scp -o StrictHostKeyChecking=no target/maven-web-application.war ec2-user@65.0.73.240:/opt/apache-tomcat-9.0.41/webapps/"    
}
}
*/
}
