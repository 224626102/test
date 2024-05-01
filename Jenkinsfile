pipeline {
    agent any
      stages {
        stage('Build') {
            steps {
                
                    echo "Compile and package code"
                    echo "Build automation tool used is Maven"
                }
            }
        
        stage('Unit and Integration Test') {
            steps {
               
                    echo "Running unit tests to ensure code funstions as expected"
                    echo "Running integration tests to ensure different components work together as expected"
                    echo "Automation tools used for this stage are JUnit and Selenium"
                }
            }
        
        stage('Code Analysis') {
            steps {
            
                    echo "Analyse code to ensure it meets industry standards"
                    echo "Tool used for this stage is SonarQube"
                    
                }
            }
        
         stage('Security scan') {
            steps {
                
                    echo "Perform a security scan on the code to identify any vulnerabilities"
                    echo "Tool used for scanning is OWASP ZAP"
                }
                post{
                    success{
                            emailext to: "fawazcom@yahoo.com",
                            subject: "Scan Successful!",
                            body: "The scan was successful!",
                            attachLog: true
                         }
                    failure{
                            mailext to: "fawazcom@yahoo.com",
                            subject: "Scan failed!",
                            body: "The scan was not successful!",
                            attachLog: true
                    }
                }
            }
        
        stage('Deploy to staging') {
            steps {
               
                    echo "Deploy the application to the testing environment"
                    echo "Tool used for this stage is AWC CodeDeploy"
                }
            }
        
        stage('Integration test on staging') {
            steps {
             
                    echo "Runnning tests to ensure application fumctions as expected in a production-like environment"
                    echo "Tool used in this stage are JUnit and Selenium"
                }
            }
        
        stage('Deploy to Production') {
            steps {
             
                    echo "Deploying the code to the production environment"
                    echo "Tool used for deployment is AWS CodeDeploy"
                }
            }
        }
    }

