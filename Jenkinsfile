pipeline {
    agent {
    dockerfile {
            filename 'Dockerfile.build'
            label 'runner-with-exifff'
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
