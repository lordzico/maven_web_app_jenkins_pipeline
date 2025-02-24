pipeline{
    agent any
    environment {
        PATH = "$PATH:/opt/apache-maven-3.9.9/bin"
    }
    stages{
       stage('GetCode'){
            steps{
				git branch: 'main',
                url: 'https://github.com/lordzico/maven_web_app_jenkins_pipeline.git'
            }
         }        
       stage('Build'){
            steps{
                sh 'mvn clean package'   
            }
         }       
    }
}
