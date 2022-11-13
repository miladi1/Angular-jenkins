pipeline {
    agent any

    stages {
        stage('Gut hub pull stage ') {
            steps {
                script{
                    checkout([$class: 'GitSCM' , branches: [[name: '*/main']] ,
                       userRemoteConfigs: [[
                           credentialsId: '6183ca82-1c90-4002-899c-bc9850c652be',
                           url :'https://github.com/miladi1/Angular-jenkins.git']]])
                }
            
            }
        }
     // stage('Build 1 ') {
       //     steps {
         //       script{
           //         
                    sh "ansible-playbook Ansible/build.yml -i Ansible/inventory/host.yml -e ansible_become_password=root "
             //   }}}
      //stage('Build 2 ') {
        //    steps {
          //      script{
            //        sh "ansible-playbook Ansible/docker.yml -i Ansible/inventory/host.yml -e ansible_become_password=root "
              //  }}}
      //stage('Build 3 ') {
        //    steps {
          //      script{
            //        sh "ansible-playbook Ansible/docker-registry.yml -i Ansible/inventory/host.yml -e ansible_become_password=root"
              //  }}}
    }
}
