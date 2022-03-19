pipeline {
  agent any
     stages {
     stage("Sync brightree API call") {
  		steps {
  			script {
				final String url = "https://betternight.com/service/v1/user/brightree/patient/sync?pwd=woRMdwN5dV@6&&limit=30"
				final String response = sh(script: "curl -s --request PUT '$url'", returnStdout: true).trim()
    			echo response
            }
        }
    }  
     
   }
   
}