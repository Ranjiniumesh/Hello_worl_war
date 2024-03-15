pipeline {
    agent {label 'slave6' }
    stages {
        stage('checkout') {
            steps {
              sh 'rm -rf hello-world-war'
            sh 'git clone https:Ranjiniumesh/Hello_worl_war.git'
            }
        }
        stage ('build') {
            steps {
                sh 'mvn --version'
                sh 'mvn clean install'
            }
        }
        stage ('deploy') {
               steps {
                   
}
}
    }
}
