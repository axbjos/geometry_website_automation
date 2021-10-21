pipeline {
    agent { 
        dockerfile { true
             args '-t geometrywebdocker:latest'
             }
        }
    stages {
        stage('test') {
            steps {
               sh 'python3 -m unittest GeometryTest.py' 
            }
        }

    }
}
