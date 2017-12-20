pipeline {
	
	agent any

	parameters {
		
			string ( name:'NAME')
		   }
	stages {

		stage('build') {
	
				steps {
						
					echo "My Branch Name: ${env.BRANCH_NAME}"
					echo "The value of the parameter is ${params.NAME}"
				      }
	
				}
		}
}
