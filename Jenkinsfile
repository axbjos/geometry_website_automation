/*declarative syntax for Docker 
*/
pipeline {
    agent any
    stages {
        stage('build') {
            steps {
               sh 'docker build --pull --rm -f "Dockerfile" -t geometrywebdocker:latest .'
            }
        }

        stage('test') {
            steps {
               sh 'docker run --rm -d  -p 5000:5000/tcp geometrywebdocker:latest'
            }
        }

        stage('deploy') {
            steps {
               sh 'docker push zrxmoto/geometrywebdocker:latest'
            }
        }

    }
}
