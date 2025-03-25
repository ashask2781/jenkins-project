pipeline {
    agent any
    parameters {
        string(name: 'ENVIRONMENT', defaultValue: 'dev', description: 'Specify environment')
        booleanParam(name: 'RUN_TESTS', defaultValue: true, description: "Hurray")
    }
    stages {
        stage('Test') {
            when {
               expression {
                        params.RUN_TESTS == true
               }
            }
            steps {
                echo "testing app"
              } 
            }
        }
        stage('Deploy') {
            steps {
                echo "deploying to ${params.ENVIRONMENT}"
            }
        }
}
