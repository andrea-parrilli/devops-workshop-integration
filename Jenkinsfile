pipeline {
    agent {
    dockerfile {
            filename 'Dockerfile.build'
            label 'dicker'
            args '-v /tmp:/tmp'
        }
     }
    stages {
        stage('build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
