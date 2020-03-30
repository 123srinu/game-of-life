def workspace; 
node
{
    //Stage is a block which defines set of tasks to perform entire the execution of job

   stage ('checkout')
   {
      //Step

checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions:
[], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'd762a279-cdd1-4668-a85e-edc2880f2a18',
url: 'https://github.com/123srinu/game-of-life.git']]])
workspace= pwd()
   }

   stage ('static code analysis')
   {
       echo "It is static code analysis"
   }
    stage ('Unit testing')
   {
       echo "Unit testing"
   }
    stage ('Delivery')
   {
       echo "Delivry"
   }

}
