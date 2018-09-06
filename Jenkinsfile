pipeline
{
	agent any
	stages{
		stage('Git') {
			steps{
			git 'https://github.com/govisr01/Maven-Demo.git'
			}
			}
		stage('Install') {
			steps{
			bat 'gradle build'
			}
			}
		stage('Deploy') {
			steps{
			sh 'cp -r "C:\\Program Files (x86)\\Jenkins\\workspace\\SBI\\Savings\\multi-module\\webapp\\target\\webapp.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps"'
			}
			}
		}
}
