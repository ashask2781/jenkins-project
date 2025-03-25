pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                echo "Welcome to testing"
              } 
            }
        stage('Deploy') {
            input {
                message "Do u want to proceed with deployment ?"
                ok "Yes Proceed"
            }
            steps {
                echo "Proceeded"
            }
        }
}
}
