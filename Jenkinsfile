node {
  stage('SCM checkout')
   {
      git 'https://github.com/devGit17/SpringMaven'
   }
   stage('compile package')
   {
     //get maven home path
     def mvnHome=tool name: 'LocalMaven', type: 'maven'
     sh "${mvnHome}/bin/mvn compile"
     echo "compiled successfully"
   }
}
