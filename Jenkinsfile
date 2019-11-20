pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'mvn -Dmaven.repo.local=/home/ubuntu/m2_repo'
                sh 'mvn -B -DskipTests clean package'
            }
        }
        stage('Test') { 
            steps {
                sh 'mvn test' 
            }
        }
    }
}
