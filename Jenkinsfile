pipeline {
    agent any
    tools { 
      maven 'maven-3' 
    }
    stages {
      stage ('Build') {
        steps {
          sh 'mvn -B -ntp -Dmaven.test.failure.ignore verify'
        }
      }

    }
}

   
