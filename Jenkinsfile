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
                echo 'Build Apps'
            }
        }
              // proses test apps
        stage('Testing Apps') {
            steps {
                echo 'Testing Apps'
            }
        }

        // Proses Scanning Apps
        stage('Scanning Apps') {
            steps {
                echo 'Scanning Apps'
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
