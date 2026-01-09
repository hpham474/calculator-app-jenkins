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
    }
}