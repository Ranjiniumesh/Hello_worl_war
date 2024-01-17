pipeline {
    agent { label 'slave6' }
    stages {
        stage('checkout') {
            steps {
              sh 'rm -rf hello-world-war'
            sh 'https://github.com/Ranjiniumesh/hello-world-war.git'
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
                   sh 'scp /home/slave6/workspace/Pipeline_01/target/hello-world-war-1.0.0.war /apache-tomcat-9.0.85/webapps'
}
}
    }
}
