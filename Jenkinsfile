// /var/lib/jenkins/tools/hudson.tasks.Maven_MavenInstallation/maven-3.9.9/bin

node 
{
   def mavenHome=tool name: "maven-3.9.9"

  stage('Git checkout')
  {
    git credentialsId: 'd5b53cfc-a0d8-4381-9e26-c06e29d8b343', url: 'https://github.com/ram251/maven-web-app-project-kk-funda.git'
  }
  
  stage('compile')
  {
   sh "${mavenHome}/bin/mvn clean compile" 
  }
  
  stage('build')
  {
   sh "${mavenHome}/bin/mvn clean package" 
  }
}
