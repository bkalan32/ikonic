pipeline {
    agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                sh 'pwd'
                sh 'cp -R helm/* .'
                sh 'ls -ltr'
                sh 'pwd'
                sh '/usr/local/bin/helm upgrade --install ikonic-app ikonic --set image.repository=bkalan322/ikonic-app --set image.tag=1'
            }           
        }
    }
}

