pipeline {
  agent any
  stages {
    stage('') {
      steps {
        parallel(
          "Repo1": {
            git 'https://github.com/bharath0080/test.git'
            
          },
          "Repo2": {
            ws(dir: '/var/tmp/Repo2') {
              git 'https://github.com/bharath0080/SampleStudentProject.git'
            }
            
            
          }
        )
      }
    }
    stage('Deploy') {
      steps {
        sh '''mvn --version;
java -version;'''
      }
    }
  }
}