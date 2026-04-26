
---

### ✅ Jenkinsfile

:::writing{variant="standard" id="fixjf"}
pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/MadihaShaikh25/CI-Workflow-Setup-using-Jenkins.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t flask-event-app .'
            }
        }

        stage('Run Container') {
            steps {
                bat 'docker run -d -p 5000:5000 flask-event-app'
            }
        }

        stage('Basic Test') {
            steps {
                bat 'curl http://localhost:5000'
            }
        }
    }
}
:::

---

# ✅ Then do:

```bash
git add .
git commit -m "fix Jenkinsfile"
git push