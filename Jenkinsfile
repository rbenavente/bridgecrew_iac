pipeline {
    agent {
        docker {
            image 'bridgecrew/jenkins_bridgecrew_runner:latest'
        }
    }
    stages {
        stage('test') {
            steps {
                script {
                    sh "/run.sh ${token} ${Repo}"

                }
            }
        }
    }
    //options {
    //    preserveStashes()
    //    timestamps()
    //    ansiColor('xterm')
    //}
}
