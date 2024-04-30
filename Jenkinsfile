pipeline {
    agent any
    environment {
        DIRECTORY_PATH = "C:\\Deakin\\Task5.1\\Jenkins_Codes_SIT753"
        TESTING_ENVIRONMENT = "TestEnv"
        PRODUCTION_ENVIRONMENT = "Fawaz Ahmed"
    }
    stages {
        stage('Build') {
            steps {
                script {
                    echo "Fetch the source code from the directory path '$DIRECTORY_PATH'"
                    echo "Compile the code and generate any necessary artifacts"
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    echo "Running unit tests"
                    echo "Running integration tests"
                }
            }
        }
        stage('Code') {
            steps {
                script {
                    echo "Check the quality of the code"
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    echo "Deploy the application to the testing environment '$TESTING_ENVIRONMENT'"
                }
            }
        }
        stage('Approval') {
            steps {
                script {
                    echo "Waiting for manual approval"
                    sleep 10
                                    }
            }
        }
        stage('Deploy to Production') {
            steps {
                script {
                    echo "Deploying the code to the production environment '$PRODUCTION_ENVIRONMENT'"
                }
            }
        }
    }
}
