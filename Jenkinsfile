peline {
  agent none
  stages {
     stage('build') {
        agent any
            steps {
                docker.build("myimage:${env.BUILD_ID}"
            }
        }
        stage('test') {
            steps {
                docker.run("myimage:${env.BUILD_ID}")
            }
        }
    }
}
