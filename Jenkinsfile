pipeline {
agent any

```
stages {

<<<<<<< HEAD
        stage('Build Docker Image') {
            steps {
                bat 'docker build -t event-registration-app .'
            }
        }

        stage('Run Docker Container') {
            steps {
                bat 'docker stop event-registration-container || exit 0'
                bat 'docker rm event-registration-container || exit 0'
                bat 'docker run -d -p 5000:5000 --name event-registration-container event-registration-app'
            }
        }

        stage('Basic Test') {
            steps {
                bat 'curl http://localhost:5000 || exit 1'
            }
=======
    stage('Build Docker Image') {
        steps {
            bat 'docker build -t event-registration-app .'
>>>>>>> parent of 36ec79a (Updated Jenkinsfile)
        }
    }

    stage('Run Docker Container') {
        steps {
            bat 'docker stop event-registration-container || exit 0'
            bat 'docker rm event-registration-container || exit 0'
            bat 'docker run -d -p 5000:5000 --name event-registration-container event-registration-app'
        }
    }

    stage('Basic Test') {
        steps {
            bat 'curl http://localhost:5000'
        }
    }
}
```

}