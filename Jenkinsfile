/*using docker pipeline steps*/
pipeline {
    agent docker
    stages {
        stage('build') {
            steps {
               docker.build("geometrywebdocker/latest") 
            }
        }

    }
}
