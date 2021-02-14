pipeline
{

agent any
   tools
    {
        maven 'M2_HOME'
    }
stages
{
   stage("checkoutcode")
    {
         steps
         {
             echo "welcome to multi-branchpipeine"
            git 'https://github.com/SriDevops-T/TestPetclinic.git'
            echo "webhooks are done"
             }
             }

   stage("check")
   {
      
       steps
      {
          echo "welcome"
      }
             }
}
}

   stage("compile the code")
   {
       steps
      {
           sh 'mvn compile'
      }
             }
}


