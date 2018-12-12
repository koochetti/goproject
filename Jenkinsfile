pipeline
	{
  	  agent any
	  
	    stages
	    {   
		stage('cloning go file')
		{
		  steps
		   {
		       sh 'mkdir -p gomain'
		       dir('gomain')
		       {
		          sh '''git clone https://github.com/koochetti/gomain.git master '''
			}
			 dir('gomain')
                       {
			  export PATH=$PATH:/goroot/bin:/gopath/bin
			  
                          sh '''go build main.go
				go run main.go'''
                        }

		   }
		}
	     }
	   }
	
