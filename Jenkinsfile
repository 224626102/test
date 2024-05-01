pipeline {
    agent any
      stages {
        stage('Build') {
            steps {
                script {
                    echo "Compile and package code"
                    echo "Build automation tool used is Maven"
                }
            }
        }
        stage('Unit and Integration Test') {
            steps {
                script {
                    echo "Running unit tests to ensure code funstions as expected"
                    echo "Running integration tests to ensure different components work together as expected"
                    echo "Automation tools used for this stage are JUnit and Selenium"
                }
            }
        }
        stage('Code Analysis') {
            steps {
                script {
                    echo "Analyse code to ensure it meets industry standards"
                    echo "Tool used for this stage is SonarQube"
                    
                }
            }
        }
         stage('Security scan') {
            steps {
                script {
                    echo "Perform a security scan on the code to identify any vulnerabilities"
                    echo "Tool used for scanning is OWASP ZAP"
                }
            }
        }
        stage('Deploy to staging') {
            steps {
                script {
                    echo "Deploy the application to the testing environment '$TESTING_ENVIRONMENT'"
                }
            }
        }
        stage('Integration test on staging') {
            steps {
                script {
                    echo "Runnning tests to ensure application fumctions as expected in a production-like environment"
                    echo "Tool used in this stage are JUnit and Selenium"
                                    }
            }
        }
        stage('Deploy to Production') {
            steps {
                script {
                    echo "Deploying the code to the production environment"
                    echo "Tool used for deployment is AWS CodeDeploy"
                }
            }
        }
    }
}
