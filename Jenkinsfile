node
 {
  
  def mavenHome = tool name: "maven3.6.3"
  
      echo "GitHub BranhName ${env.BRANCH_NAME}"
      echo "Jenkins Job Number ${env.BUILD_NUMBER}"
      echo "Jenkins Node Name ${env.NODE_NAME}"
  
      echo "Jenkins Home ${env.JENKINS_HOME}"
      echo "Jenkins URL ${env.JENKINS_URL}"
      echo "JOB Name ${env.JOB_NAME}"
  
 
stage('checkoutcode')
{
git branch: 'development', credentialsId: '3620f580-d3ca-4f5d-8d66-3f0956472699', url: 'https://github.com/Murali-Grahitha-org/maven-web-application.git'
}
stage('build')
{
sh "${mavenhome}/bin/mvn clean package"
 
/*
 stage("ExecuteSonarQubeReport")
 {
 sh "${mavenHome}/bin/mvn sonar:sonar"
 }
 
 stage("UploadArtifactsintoNexus")
 {
 sh "${mavenHome}/bin/mvn deploy"
 }
 
  stage("DeployAppTomcat")
 {
  sshagent(['423b5b58-c0a3-42aa-af6e-f0affe1bad0c']) {
    sh "scp -o StrictHostKeyChecking=no target/maven-web-application.war  ec2-user@15.206.91.239:/opt/apache-tomcat-9.0.34/webapps/" 
  }
 }
 
 stage('EmailNotification')
 {
 mail bcc: 'devopstrainingblr@gmail.com', body: '''Build is over

 Thanks,
 Mithun Technologies,
 9742011456.''', cc: 'devopstrainingblr@gmail.com', from: '', replyTo: '', subject: 'Build is over!!', to: 'devopstrainingblr@gmail.com'
 }
 */
 
 }
