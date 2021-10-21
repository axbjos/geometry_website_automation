/*declarative syntax for Docker 
*/
pipeline {
    stages {
        stage('build') {
            steps {
               sh 'docker build --pull --rm -f "Dockerfile" -t geometrywebdocker:latest' 
            }
        }

    }
}
