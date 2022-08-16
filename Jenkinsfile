pipeline {
    agent any
    environment {
        PATH="/opt/maven/bin:$PATH"
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Hi') {
            steps {
                echo 'I am shivasai'
            }
        }
        stage('Task') {
            steps {
                echo 'Run the build job'
            }
        }
        stage('SCM') {
            steps {
                git 'https://github.com/Shivasai011/hello-world.git'
            }
        }
        stage('Build') {
            steps {
                sh "mvn package"
            }
        }
    }
}
