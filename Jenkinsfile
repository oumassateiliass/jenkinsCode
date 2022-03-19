pipeline {
  agent any
     stages {
     stage("Sync easypost trackers") {
  		steps {
  			script {
				final String url = "https://betternight.com/service/v1/order/trackers/sync?pwd=Dq0eYZ@M3Zl0"
				final String response = sh(script: "curl -s --request GET $url", returnStdout: true).trim()
    			echo response
            }
        }
    }  
     
   }
   
}