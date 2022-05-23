
pipeline {
    agent any
    stages {
        stage ('Compile ')
{
steps
 {
      withMaven (maven: 'MAVEN-HOME')
{
bat 'mvn compile'
}
}
}
        stage('Test') {
            steps {
            
      withMaven (maven: 'MAVEN-HOME')
      {
                echo 'Testing..'
                bat 'mvn test'
            }
        }
        }
        
        stage('packaging') {
            steps {
            
      withMaven (maven: 'MAVEN-HOME')
      {
                echo 'Testing..'
                bat 'mvn package'
            }
        }
        }
        }
    } 


