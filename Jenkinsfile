pipeline {
    agent { 
        dockerfile {
             label 'geometrydocker'
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
