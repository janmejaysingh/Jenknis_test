pipeline {
	agent any
	triggers { cron('0 16 * * *') }
	stages {
		stage("Get SCM branches") {
			steps {
				script {
				echo "This is Get SCM branches "
				println env.JOB_NAME
				println env.BUILD_NUMBER
				// echo %BUILD_NUMBER%
				// println "JOB_NAME: " + System.getenv("JOB_NAME")
				// println "BUILD_NUMBER: " + System.getenv("BUILD_NUMBER")
				}
				//echo %BUILD_NUMBER%
			}
		 }
		 
		stage("Get User Input") {
			steps {
                  script {
				echo "this is Get User Input"
				}
			}
		 }

		stage("Checkout selected branch") {
			steps {
			script {
				echo "this is Checkout selected branch"
				}
			}
		 }

		stage("Deploy to OpenShift") {
			steps{
            	script {
				echo "This is Deploy to OpenShift"
				}
        	}
		}
		 
	 }
}
