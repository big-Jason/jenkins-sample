pipeline {
  agent any
  stages {
    stage('ansible Step') {
        steps{
          dir(path: 'ansible') {
            ansiColor(colorMapName: 'xterm') {
              ansiblePlaybook(
                playbook: 'playbook.yml',
#                inventory: 'inventory',
                colorized: true)
            }
          }
        }
    }
  }
}