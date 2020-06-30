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
          echo "Test run successfully"
         }}
   }
    post{
         always{
            emailext body: 'This is QA env build', subject: 'QA Build success', to: 'absharmam@gmail.com'
         }
      }
}
