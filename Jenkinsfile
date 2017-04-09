node {
   
   	stage 'Stage 1'
      node{
   		echo 'Hello there, shell scripts'
      }

   	stage 'Checkout'
      node{
   		git url: 'https://github.com/lzhengqc/jenkins-pipeline-shell-scripts.git'
      }

   	stage 'Permission Setting'
      node{
   		sh 'chmod +x *.sh'
      }

   	stage 'Build'
      node{
   		sh './myBuild.sh'   	
      }

   	stage 'Test'
      node{
   		sh './myTest.sh'
      }

   	stage 'Deploy'
      node{
   		sh './myDeployment.sh'
      }
}