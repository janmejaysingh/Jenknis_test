pipeline {
	agent any
	triggers { cron('H/5 * * * *') }
	stages {
		stage("Get SCM branches") {
			steps {
				script {
				echo "This is Get SCM branches "
				echo %BUILD_NUMBER%
				println "JOB_NAME: " + System.getenv("JOB_NAME")
				println "BUILD_NUMBER: " + System.getenv("BUILD_NUMBER")
				}
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
