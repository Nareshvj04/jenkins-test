pipeline {
    agent { label 'built-in'}

    stages {
        stage('Clone') {
            steps {
                git branch: 'main',
                url: 'https://github.com/Nareshvj04/jenkins-test.git'
            }
        }
        stage('Run Python Script') {
            steps {
                // This executes the python file you just cloned
                sh 'python3 sample.py' 
            }
        }

        stage('Build') {
            steps {
                echo 'Building application...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running unit tests...'
            }
        }
    }
}
