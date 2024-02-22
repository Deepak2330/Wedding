pipeline{
   agent any
   stages{
	stage('clean workspace')
	{
           steps{
              sh ' rm -r *'
	      sh ' rm -r ../../../../www/html/*'
	   }
	}

        stage('git scm clone'){
             
	     steps{
                  
		  sh ' git clone https://gitlab.com/9901845901dk/wedding.git -b beta '

	     }
 
	}
	stage('deploy'){
              steps{
                sh 'mv wedding/* ../../../../www/html'
	      }
	}
     
   }
  
}
