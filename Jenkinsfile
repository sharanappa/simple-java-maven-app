pipeline  {
agent any    
stages {
        stage('Build') {
            steps {
                   sh ./jenkins/scripts/build.sh
            }

        }
        stage('Test') {
            steps {
                    sh ./jenkins/scripts/tesh.sh 
            }
        }
        stage('Deliver') { 
            steps {
                ./jenkins/scripts/deliver.sh 
            }
        }

}    }
}
