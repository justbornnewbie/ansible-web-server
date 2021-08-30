pipeline{
    agent{
        label "worker1"
    }
    stages{
        stage("install-nginx"){
            steps{
                sh '''
                ansible-playbook -i host nginx-ansible.yml
                '''
            }
        }
    }
}