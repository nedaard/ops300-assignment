pipeline {
    agent { label 'c1-agent' }

    stages {
        stage('Build') {
            steps {
                sh '''
                podman build -t registry.assign.nardebilian.300.ops:5000/web:${BUILD_NUMBER} .
                '''
            }
        }
    }
}
