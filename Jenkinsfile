pipeline {
  agent any
  
  stages {
    stage('checkout stage') {
      steps {
        sh 'rm -rf grafana'
        sh 'git clone https://github.com/Chaitraradha/grafana.git'
      }
    }
    stage('running playbook') {
      steps {
        sh 'ansible-playbook -i hosts graf.yml'
      }
    }
  }
}
