pipeline {
    agent {
        label 'XYZ'
        }

    stages {
        stage('Build Image') {
            steps {
                sh 'sudo docker build -t desaiakshay92/flask_jenkins .'
            }
        }
        stage('Run Image') {
            steps {
                sh 'sudo docker run -d --name flask_container desaiakshay92/flask_jenkis'
            }
        }
        stage('Test') {
            steps {
                echo 'Successfully Pushed'
            }
        }
    }
}
