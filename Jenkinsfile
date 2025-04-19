pipeline {
    agent any
        tools {
        maven 'Maven' // Optional: remove if not using Maven
    }
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/Surya-coder-23/pipeline-scm.git', branch: 'main'  // clone the repository
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }


     }
 }  
 }
}


