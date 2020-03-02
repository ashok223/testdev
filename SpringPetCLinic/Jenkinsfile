node {
    
    stage('SCM') {
         // git clone    
         git 'https://github.com/ashok223/spring-petclinic.git'
  }
     stage ('build the packages') {
      // mvn package
        sh 'mvn package'
  }
  stage ('show test results') {
      // unit testing
        junit 'target/surefire-reports/*.xml'

  }
     stage ('archival') {
      // archiving artifacts
        archive 'target/*.jar'
  }
  
 }