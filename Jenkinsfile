pipeline
	{
  	  agent any
	  {
	    stages
	    {
		stage('cloning go file')
		{
		  steps
		   {
		       sh 'mkdir -p gomain'
		       dir('gomain')
		       {
		          sh ''' https://github.com/koochetti/gomain.git '''
			}
			 dir('gomain')
                       {
                          sh '''go run main.go'''
                        }

		   }
		}
	     }
	   }
	}
