pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Task: Compile and package the source code.'
                echo 'Tool: Maven'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Task: Run unit tests and integration tests to verify code and component behavior.'
                echo 'Tool: JUnit (unit), Postman/Newman (integration)'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Task: Analyse code quality and maintainability against industry standards.'
                echo 'Tool: SonarQube / SonarCloud'
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Task: Scan the code and dependencies for known vulnerabilities.'
                echo 'Tool: OWASP Dependency-Check / Snyk'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Task: Deploy the application to a staging server for pre-production testing.'
                echo 'Tool: AWS EC2 (via SSH/SCP or AWS CLI)'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Task: Run integration tests against the staging environment to confirm production-like behaviour.'
                echo 'Tool: Selenium / Postman'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Task: Deploy the verified application build to the production server.'
                echo 'Tool: AWS EC2 (via SSH/SCP or AWS CLI)'
            }
        }
    }
}
