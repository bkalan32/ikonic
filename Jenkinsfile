pipeline {
    agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                sh 'pwd'
                sh 'cp -R helm/* .'
                sh 'ls -ltr'
                sh 'pwd'
                sh '/usr/local/bin/helm upgrade --install petclinic-app ikonic --set image.repository=hub.docker.com/repository/docker/bkalan322/ikonic-app --set image.tag=1'
            }           
        }
    }
}

