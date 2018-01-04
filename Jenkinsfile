pipeline {
	
	agent {

		docker 'ant-image'
	      }

	parameters {
		
			string ( name:'NAME')
			booleanParam ( name:'PRINT')

		   }
	stages {

		stage('build') {
	
				steps {
				
						sh 'ant -f build.xml -v'		
				      }
	
				}

	stage('test') {
                                steps {
                                                sh 'ant -f test.xml -v'
                                      }
                       }        
		}
}
