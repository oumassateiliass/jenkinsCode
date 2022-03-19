pipeline {
  agent any
     stages {
     stage("Sync Snapmd appointments") {
  		steps {
  			script {
				final String url = "https://betternight.com/service/v1/consult/appointments/sync?pwd=jfPl@pKrKiZB"
				final String response = sh(script: "curl -s --request GET $url", returnStdout: true).trim()
    			echo response
            }
        }
    }  
     
   }
   
}