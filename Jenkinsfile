pipeline {
	agent any
	triggers { cron('H/5 * * * *') }
	stages {
		stage("Get SCM branches") {
			steps {
				script {
				echo "This is Get SCM branches "
				println env.JOB_NAME
				println env.BUILD_NUMBER
				println env.BUILD_ID
				println env.BUILD_DISPLAY_NAME
				println env.JOB_NAME
				println env.JOB_BASE_NAME
				println env.BUILD_TAG
				println env.EXECUTOR_NUMBER
				println env.NODE_NAME
				println env.NODE_LABELS
				println env.WORKSPACE
				println env.JENKINS_HOME
				println env.JENKINS_URL
				println env.BUILD_URL
				println env.JOB_URL
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
