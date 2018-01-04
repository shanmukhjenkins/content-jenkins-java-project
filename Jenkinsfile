pipeline {

	tools{
		ant 'Ant_1,10,1'

	     }
	
	agent {

		docker 'centos'
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
