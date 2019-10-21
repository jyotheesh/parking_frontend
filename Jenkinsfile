node('master'){
	   stage('git checkout'){
	                  git 'https://github.com/mythribhay/Inglibraryui'
	              }
	   stage('angular build'){
		     sh '''
	             npm install
	             ng build
		     '''
	         }
	
	}
