node() {
        stage('Build') {
                sh '/opt/maven/bin/mvn clean package'
        }
        stage('Test') {
                sh '/opt/maven/bin/mvn test'
            }
        stage('Deliver') { 
                sh './jenkins/scripts/deliver.sh' 
        }
}
