node() {
    stages {
        stage('Build') {
            steps {
                sh '/opt/maveen/bin/mvn clean package'
            }
        }
        stage('Test') {
            steps {
                sh '/opt/maveen/bin/mvn test'
            }
            post {
                always {
                    junit 'target/surefire-reports/*.xml'
                }
            }
        }
        stage('Deliver') { 
            steps {
                sh './jenkins/scripts/deliver.sh' 
            }
        }
    }
}
