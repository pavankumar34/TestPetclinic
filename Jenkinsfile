Multi-branch pipeline:
_______________________
for every branch---job-in jenkins--
developement-----bracnh-jenkins --
release
test
bugfix
Master

jenkinsfile------------>must be inside soource code tree--github
inputfile-Jenkindfile

ALLOWS US TO AUTOMATICALLY CREATE A PIPELINE FOR EACH BRANCH ON YOU SOURCODE REPOSITORY WITH TH HELP OF JENKINS FILE

jenkinsfile---pipeline as acode




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
  sh 'mvn package'

}
}
