pipeline {
    agent any
 

    
    stages{
        stage("git pull"){
            steps{
              
                git branch: 'main', 
                credentialsId: '7a11751d-b52e-4b05-9c01-6c8ab6bd2941', 
                url: 'https://github.com/miladi1/Angular-jenkins.git'
                    
                }
                
            }
      
//          stage("Build"){
//             steps{
              
//               script {
//                  sh  "ansible-playbook ansible/build.yml -i ansible/inventory/host.yml"
//               }
//             }
// //          }
//       
      
// //           stage("Docker"){
//             steps{
//               
//             
//                  sh  " ansible-playbook ansible/docker.yml -i ansible/inventory/host.yml"
// //               
//             }
//          }
//        stage('docker-registry'){
//             steps{
//                 script{
//                     sh "ansible-playbook ansible/docker-registry.yml -i ansible/inventory/host.yml "
//                 }
//             }
//         }
//       
//     

	}

}
