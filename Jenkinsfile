#!groovy

node('localhostt')  {
agent any   
stages {
        stage('Build') {
            steps {
                script {

                   sh '/home/sharan/jenkins_maveen_example/simple-java-maven-app/jenkins/scripts/build.sh'
             }
            }

        }
        stage('Test') {
            steps {
                script {
                    sh '/home/sharan/jenkins_maveen_example/simple-java-maven-app/jenkins/scripts/tesh.sh' 
               }

            }
        }
        stage('Deliver') { 
            steps {
               script {
                sh '/home/sharan/jenkins_maveen_example/simple-java-maven-app/jenkins/scripts/deliver.sh'
             }
            }
        }

}    
}
