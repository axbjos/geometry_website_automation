/*declarative syntax for Docker 
*/
pipeline {
    agent any
    stages {
        stage('build') {
            steps {
               sh 'docker build --pull --rm -f "Dockerfile" -t geometrywebdocker:latest' 
            }
        }

    }
}
