pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git 'https://github.com/PabloNS/demo-jenkins.git'

                sh "./mvnw clean package"

                sh "./mvnw spring-boot:run"
            }
        }
    }
}