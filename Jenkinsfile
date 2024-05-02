pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // sh 'mvn --version'
                // sh 'node --version'
                echo 'Build'
                // Whats the path
                echo "Path: $PATH"
                // What"s the build number
                echo "Build Number: $env.BUILD_NUMBER"
                // Whats the build id
                echo "Build ID: $env.BUILD_ID"
            }
        }
        stage('Test') {
            steps {
                echo 'Test'
            }
        }
        stage('Integration Test') {
            steps {
                echo 'Integration Test'
            }
        }
    }
    post {
        always {
            echo 'I always run'
        }
        success {
            echo 'I run when successful'
        }
        failure {
            echo 'I run when failed'
        }
	}
}