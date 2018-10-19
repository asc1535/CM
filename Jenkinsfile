pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                sh 'mvn clean -DskipTest -U package' 
            }
        }
        stage('Deploy') {
            steps {
                sh 'mvn -DskipTest deploy'
            }
        }
    }
}
