pipeline {
    agent any
    stages {
        stage('Project Details') {
            steps {
                echo "==========================================="
                echo "   Calculator Freestyle Build"
                echo "==========================================="
                echo "Build Number: ${BUILD_NUMBER}"
                echo "Workspace: ${WORKSPACE}"
                sh 'echo "Date: ${date}"'
                echo "==========================================="
                echo "Project files:"
                sh "ls -la"
            }
        }
        stage('Build') {
            steps {
                echo "Building application..."
                sh 'chmod +x mvnw'

                sh './mvnw --version'

                sh './mvnw clean compile -B'

                echo "Compilation successful!"
            }
        }
    }
}