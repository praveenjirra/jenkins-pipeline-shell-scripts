node {
   
   	stage 'Stage 1'
   		echo 'Hello there, shell scripts'
   	stage 'Checkout'
   		git url: 'https://github.com/lzhengqc/jenkins_pipeline_shell_scripts'
   	stage 'Permission Setting'
   		sh 'chmod +x *.sh'
   	stage 'Build'
   		sh './myBuild.sh'   	
   	stage 'Test'
   		sh './myTest.sh'
   	stage 'Deploy'
   		sh './myDeployment.sh'
  
}
