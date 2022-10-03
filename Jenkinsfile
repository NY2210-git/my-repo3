pipeline {
     
	   agent {
	          
			  label '172.31.15.40'
			  
			  }
	    
		stages {

                stage ('httpd-instsa'){

                    steps {
   
                         sh " sudo yum install httpd -y"
          
                          }

                       }
					   
					    stage ('httpd-start'){

                    steps {
   
                         sh " sudo service httpd start"
          
                          }

                       } 
					   
					   stage ('index-dep'){

                    steps {
   
                         sh " sudo cp -r index.html /var/www/html"
						  sh " sudo chmod 777 /var/www/html/index.html"
						 
          
                          }

                       }
					   
              
			  }


}
