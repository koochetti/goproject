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
			  
			  
                          sh '''export PATH=$PATH:/goroot/bin:/gopath/bin
			  go build main.go
				go run main.go'''
                        }

		   }
		}
	     }
	   }
	
