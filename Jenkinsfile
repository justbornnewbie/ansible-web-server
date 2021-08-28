pipeline{
    agent {
        label: ansibleworker1
    }
    stages{
        stage("install-httpd"){
            steps{
                sh '''
                ansible-playbook -v 5 -i host http-ansible.yml
                '''
            }
        }
    }
}