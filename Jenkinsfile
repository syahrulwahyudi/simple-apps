pipeline {
    //job akan dijalankan pada agent devops1-syahrul
    agent {
        node {
            label'devops1-syahrul' 
    // some block
            }
        }

   // proses sdlc
    stages {
        // proses build apps
        stage('Build Apps') {
            steps {
                sh 'npm install'
            }
        }

       // proses copy environtment variable
        stage('Copy env') {
            steps {
                sh 'cp -p /home/ubuntu/Hari-1/simple-apps/.env .'
            }
        }

              // proses test apps
        stage('Testing Apps') {
            steps {
                sh 'npm test'
            }
        }

        // Proses Scanning Apps
        stage('Scanning Apps') {
            steps {
                sh  'sonar-scanner   -Dsonar.projectKey=simple-apps   -Dsonar.sources=.   -Dsonar.host.url=http://172.23.5.11:9000   -Dsonar.login=sqp_61a10a093e71b82d7085e81dfd855c43c9257f75'
            }
        }
        // Proses Build Image
        stage('Build Image') {
            steps {
                echo 'Build Image'
            }
        }

       // Proses deploy apps
        stage('Deploy Apps') {
            steps {
                echo 'Deploy Apps'
            }
        }

      // Proses publish image
        stage('Publish Image') {
            steps {
                echo 'Publish Image'
            }
        }
    }
}
