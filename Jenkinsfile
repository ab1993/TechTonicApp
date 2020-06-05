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
         }}
      post{
         always{
            emailext body: 'Hi new build deployed successfully', recipientProviders: [developers()], subject: 'QA ENV BUILD', to: 'absharmasb@gmail.com'
         }
      }
   }
}
