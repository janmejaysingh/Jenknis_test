pipeline {
	stages {
		stage("Get SCM branches") {
			steps {
				script {
				echo "This is Get SCM branches"
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