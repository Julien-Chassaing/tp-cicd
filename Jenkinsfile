pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository

                // Run Maven on a Unix agent.
                //sh "mvn -Dmaven.test.failure.ignore=true clean package"

                // To run Maven on a Windows agent, use
                bat "mvn -Dmaven.test.failure.ignore=true clean package"
            }

            post {
                // If Maven was able to run the tests, even if some of the test
                // failed, record the test results and archive the jar file.
                success {
<<<<<<< HEAD
                    junit '*/target/surefire-reports/TEST-cicd.learn.tp1.AppTest.xml'
=======
                    junit '*/target/surefire-reports/TEST-.xml'
>>>>>>> develop
                    archiveArtifacts 'target/*.jar'
                }
            }
        }
    }
}
