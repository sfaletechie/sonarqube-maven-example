pipeline {
    agent any
    stages {
        stage("Clone code from GitHub") {
            steps {
                script {
                    git branch: 'master', url: 'https://github.com/rajulucky812/sonarqube-maven-example.git';
                }
            }
        }
        stage("Maven sonar") {
            steps {
                script {
                    sh "mvn sonar:sonar -Dsonar.host.url=http://localhost:9000 -Dsonar.login=5beebd596d0c952cd460c3e7e9f1e1ce2d878266"
                }
            }
        }				
		}
        }
