#!groovy
@Library('jenkins-shared-library@master') _

pipeline {
    agent any

    parameters {
      string(name: "DEV_TO_TEST_EXPORT_API_URL", defaultValue: "", description: "Export API URL for dev to test environment promotion")
      string(name: "DEV_TO_TEST_EXPORT_API_CREDENTIAL", defaultValue: "<username>:<password>", description: "Export API Credential for dev to test environment promotion")      
    }

    stages {
        stage('Promote Forms In A File') {
            steps {
              promoteForms()
            }
        }
    }
}