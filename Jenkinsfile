pipeline
{

agent any
stages
{
   stage("checkoutcode")
    {
         steps
         {
             echo "welcome to multi-branchpipeine"
            git 'https://github.com/SriDevops-T/TestPetclinic.git'
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
}
