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
				      }
				when {
				
					expression {
							
							params.PRINT=="True"
						   }
				     }

				steps {

					echo "The value of the parameter is ${params.NAME}"
				      }
	
				}
		}
}
