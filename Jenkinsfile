pipeline {
   agent any
  
   stages {
      stage('Build') {
         steps {
            // Get some code from a GitHub repository
            git 'https://github.com/ApiseroAnand/test2.git'
            // To run Maven on a Windows agent, use
            bat "mvn -Dmaven.test.failure.ignore=true clean package"
         }
      }
      stage('Test') {
         steps {
            // Get some code from a GitHub repository
            git 'https://github.com/ApiseroAnand/test2.git'
            // To run Maven on a Windows agent, use
             bat "mvn -Dmaven.test.failure.ignore=true clean test"
         }
      }
      stage('Deploy') {
         steps {
            // Get some code from a GitHub repository
            git 'https://github.com/ApiseroAnand/test2.git'
            // To run Maven on a Windows agent, use
             bat "mvn -Dmaven.test.failure.ignore=true clean deploy -DmuleDeploy"
         }
      }
   }
}
