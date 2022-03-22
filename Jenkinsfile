pipeline {
  agent any
     stages {
     stage("Sync easypost trackers") {
	environment {
         rechu_Username = credentials('JENKINS_USERNAME')
       }
  		steps {
		sh(script: "echo 'my username is $rechu_Username_USR'")
                sh(script: "echo 'my password is $rechu_Username_PSW'")
  			script {
				final String url = "https://betternight.com/service/v1/order/trackers/sync?pwd=Dq0eYZ@M3Zl0"
				final String response = sh(script: "curl -s --request GET $url", returnStdout: true).trim()
    			echo response
            }
        }
    }  
     
   }
   
}
