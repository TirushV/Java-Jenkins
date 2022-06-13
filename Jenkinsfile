pipeline  {
    agent any
    stages  {
        stage("GitClone") {
            steps {
                git 'https://github.com/TirushV/Java-Jenkins.git'
            }
        }
        stage("Build") {
            steps {
                tool name: 'maven', type: 'maven'
                sh "mvn clean install"
            }
        }
    }
}
