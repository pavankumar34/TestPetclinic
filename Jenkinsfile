pipeline
{

agent any
   tools
    {
        maven 'MAVEN'
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



   stage("compile the code")
   {
       steps
      {
           sh 'mvn compile'
      }
             }
stage("test")
{
 steps
{
   sh 'mvn test'

}
}

stage("package")
{
   steps
   {
  sh 'mvn package'
   }

}
}
}

