Jenkinsfile (Declarative Pipeline)
pipeline{
    agent any
    tools{
        gradle "Gradle-6"
    }
    stages { 
        stage('clone repository') {
          steps { 
            git 'https://github.com/kahenya-anita/gallery'
          }
        }
        stage('Build project') {
          steps { 
            sh 'gradle build'
          }
        }
        stage('Tests'){
            steps {
                sh 'gradle test'
            }
        }
  }
}