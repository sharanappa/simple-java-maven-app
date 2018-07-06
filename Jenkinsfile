node() {
        stage('Build') {
                sh '/opt/maveen/bin/mvn clean package'
        }
        stage('Test') {
                sh '/opt/maveen/bin/mvn test'
            }
        stage('Deliver') { 
                sh './jenkins/scripts/deliver.sh' 
        }
}
