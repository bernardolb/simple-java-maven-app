pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
                sh 'echo Oi > /tmp/malware.out' 
            }
        }
    }
}
