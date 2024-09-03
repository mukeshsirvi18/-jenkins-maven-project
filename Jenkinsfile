pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Run Maven from the correct directory where pom.xml is located
                dir('hello-app') {
                    sh 'mvn clean package'
                }
            }
        }

        stage('Test') {
            steps {
                // Run tests
                dir('hello-app') {
                    sh 'mvn test'
                }
            }
        }
    }
}
