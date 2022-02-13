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
        ansiblePlaybook(playbook: 'ansible-httpd-install.yml', become: true, credentialsId: '68dc4bbc-5743-4186-8b87-2f552c36148d', disableHostKeyChecking: true)
      }
    }

  }
}