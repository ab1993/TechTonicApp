pipeline{
   agent any
   stages{
       stage("checkout the code"){
          steps{
          git "https://github.com/ab1993/TechTonicApp.git"
          } }
       stage("QA env"){
         steps{
          echo "qa run successfully"
         }
      }
   }
}
