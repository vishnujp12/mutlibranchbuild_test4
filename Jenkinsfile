pipeline {
    agent {
        docker {
            //image 'buildcontainer:2.7'
            //image 'buildcontainer:3.3' use this
            image 'buildcontainer:3.5'

        }
    }

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code inside the Docker container
                checkout scm
            }
        }

        stage('Build') {
            steps {
                // Run the Python script without changing the directory
                //sh "python3 /app/g3.py"
                sh "python3 /app/g4.py"

                
            }
        }
    }
}
