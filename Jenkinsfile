pipeline {
  agent any
     stages {
     stage("Sync Snapmd consult reports") {
  		steps {
  			script {
				final String url = "https://betternight.com/service/v1/consult/snapmd/reports/sync?pwd=jfPl@pKrKiZB"
				final String response = sh(script: "curl -s --request GET $url", returnStdout: true).trim()
    			echo response
            }
        }
    }  
     
   }
   
}