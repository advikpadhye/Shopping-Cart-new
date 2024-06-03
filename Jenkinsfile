pipeline {
    agent any
    tools {
        maven 'maven3'
        jdk 'jdk17'
    }
        stage('Compile the Code') {
            steps {
              sh "mvn clean compile"
            }
        }
        
        stage('test the Code') {
            steps {
              sh "mvn clean test"
            }
        }
        
        
        stage('package the Code') {
            steps {
              sh "mvn clean package"
            }
        }
        
    }
}
