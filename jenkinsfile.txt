pipeline
{
agent any
stages
{
 stage('Commit')
 {
  steps
  {
   echo "Source Code Download from the GITHUB to Declarative Pipeline......."
  }
 } 
 stage('Build')
 {    
  steps
   {
    echo "This is Build project run with maven tool ................"
   }
  }
 stage('Test')
 {
  steps
  {
    echo "This is Test project run with Selenium tool ................"
  }
 } 
 stage('Deploy')
 {    
  steps
   {
    echo "This is Deploy project run with Docker tool ................"
   }
  }
 stage('Monitor')
 {    
  steps
   {
    echo "This is Monitoring project run with Splunk tool ................"
   }
  }
}
}
