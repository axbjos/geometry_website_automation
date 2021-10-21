/*using docker pipeline steps*/
pipeline {
    agent { any }
    stages {
        stage('build') {
            steps {
               docker.build("geometrywebdocker/latest") 
            }
        }

    }
}
