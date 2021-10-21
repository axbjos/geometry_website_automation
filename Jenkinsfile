/*declarative syntax for Docker 
*/
pipeline {
    agent none
    stages {
        stage('build') {
            steps {
               sh 'docker build --pull --rm -f "Dockerfile" -t geometrywebdocker:latest' 
            }
        }

    }
}
