<<<<<<< HEAD
=======
/* groovylint-disable-next-line CompileStatic */
>>>>>>> a2c2d4b (first)
pipeline {
    agent any

    environment {
<<<<<<< HEAD
        CONTAINER_IMAGE  = 'nestjs_image' // Replace with your Docker Hub credentials ID
        CONTAINER_NAME   = 'nestjs_container'
        PORT             = '3000'
=======
        CONTAINER_IMAGE = 'nestjs_image'
        CONTAINER_NAME  = 'nestjs_container'
        PORT            = '3000'
>>>>>>> a2c2d4b (first)
    }

    stages {
        stage('Clone Repository') {
            steps {
<<<<<<< HEAD
                git branch: 'main', url: 'https://github.com/mohsinakhtaralam/nestproject.git'
            }
        }

        stage('Docker container image build') {
            steps {
                
                    sh "docker build -t ${CONTAINER_IMAGE} ."
               
            }
        }

        stage('Stop and Remove Existing Container') {
            steps {
                sh """
                    docker stop ${CONTAINER_NAME} || true
                    docker rm ${CONTAINER_NAME} || true
                """
            }
        }
        stage('start container') {
            steps {
               
                    sh "docker run -d --name ${CONTAINER_NAME} -p ${PORT}:${PORT} ${CONTAINER_IMAGE}"
               
        }
    }
}
}
=======
               git branch: 'main', url: ''
            // Add your build steps here
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            // Add your test steps here
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            // Add your deploy steps here
            }
        }
    }

    post {
        always {
            echo 'This will always run after the stages.'
        }
        success {
            echo 'This will run only if the pipeline succeeds.'
        }
        failure {
            echo 'This will run only if the pipeline fails.'
        }
    }
}
>>>>>>> a2c2d4b (first)
