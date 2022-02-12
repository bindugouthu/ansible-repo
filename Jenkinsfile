pipeline {
  agent any

  stages {
    stage('ansible version') {
      steps {
        sh '''
          ansible --version
          ansible-playbook --version
          ansible-galaxy --version
        '''
      }
    }
  }
}
