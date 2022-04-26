pipeline {
    agent {
        label 'centos'
    }
    stages {
        stage('requirements') {
            steps{
               sh "pip3 install -r tox-requirements.txt" 
               sh "ansible-galaxy collection install community.docker"
               sh "ansible-galaxy collection install community.general"
            }
        }
        stage('molecule'){
            steps{
                sh "molecule test"
            }
        }
    }
}
