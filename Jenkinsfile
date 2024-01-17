pipeline {
    agent { label 'slave6' }
    stages {
        stage('checkout') {
            steps {
              sh 'rm -rf hello-world-war'
              sh '
                echo 'Hello World'
            }
        }
    }
}
