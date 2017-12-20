pipeline {
	
	agent any

	parameters {
		
			string ( name:'NAME')
			booleanParam ( name:'PRINT')

		   }
	stages {

		stage('build') {
	
				steps {
						
					echo "My Branch Name: ${env.BRANCH_NAME}"
					echo "The value of the parameter is ${params.PRINT}"
				      }
	
				}

		stage('test') {
				when {
				
					allOf {
						expression { params.PRINT ==~ /(?i)(TRUE)/ }
						expression { params.NAME == 'Sai Shanmukh' }
					      }
				     }

				steps {

					echo "The value of the parameter is ${params.NAME}"
				      }
	
				}
		}
}
