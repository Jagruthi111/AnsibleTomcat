pipeline {
  agent any
  
  stages {
    stage('checkout stage') {
      steps {
        sh 'rm -rf AnsibleTomcat'
        sh 'git clone https://github.com/Jagruthi111/AnsibleTomcat.git'
      }
    }
    stage('running playbook') {
      steps {
        sh 'ansible-playbook -i hosts demo.yml'
      }
    }
  }
}
