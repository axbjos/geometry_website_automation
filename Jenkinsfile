pipeline {
    agent { dockerfile true}

    stages {
        stage('test') {
            steps {
               sh 'python3 -m unittest GeometryTest.py' 
            }
        }

    }
}