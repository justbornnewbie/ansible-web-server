pipeline{
    agent{
        label "worker1"
    }
    stages{
        stage("install-httpd"){
            steps{
                sh '''
                ansible-playbook -i host http-ansible.yml
                '''
            }
        }
    }
}