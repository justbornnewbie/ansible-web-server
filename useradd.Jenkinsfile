pipeline{
    agent{
        label "worker1"
    }
    stages{
        stage("useradd"){
            steps{
                sh '''
                ansible-playbook useradd.yaml
                '''
            }
        }
    }
}