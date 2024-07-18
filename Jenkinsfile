pipeline{
    agent any
    tools{
        maven 'maven'
    }
    stages{
        stage('pull src'){
            steps{
                git 'https://github.com/niveditanivvi/webapp2.git'
            }
        }
        stage('clean'){
        steps{
            sh 'mvn clean'
        }
    }
     stage('validate'){
        steps{
            sh 'mvn validate'
        }
    }
     stage('compile'){
        steps{
            sh 'mvn compile'
        }
    }
     stage('test'){
        steps{
            sh 'mvn test'
        }
    }
     stage('package'){
        steps{
            sh 'mvn package'
        }
    }
}
}
