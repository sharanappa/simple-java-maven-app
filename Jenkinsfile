#!groovy

pipeline  {
agent any    
stages {
        stage('Build') {
            steps {
                script {

                   sh './jenkins/scripts/build.sh'
             }
            }

        }
        stage('Test') {
            steps {
                script {
                    sh './jenkins/scripts/tesh.sh' 
               }

            }
        }
        stage('Deliver') { 
            steps {
               script {
                sh './jenkins/scripts/deliver.sh'
             }
            }
        }

}    
}
