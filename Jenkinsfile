#!groovy​
node {
   
   	stage('Stage 1'){
   		echo 'Hello there, shell scripts'
      }

   	stage('Checkout'){
   		git url: 'https://github.com/lzhengqc/jenkins-pipeline-shell-scripts.git'
      }

   	stage('Permission Setting'){
   		sh 'chmod +x *.sh'
      }

   	stage('Build'){
   		sh './myBuild.sh'   	
      }

   	stage('Test'){
   		sh './myTest.sh'
      }

   	stage('Deploy'){
         input 'Do you approve deployment?'
         
   		sh './myDeployment.sh'
      }
}