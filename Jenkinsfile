pipeline {
     
	   agent {
	          
			  label 'built-in'
			  
			  }
	    
		stages {

                stage ('httpd-inst'){

                    steps {
   
                         sh "yum install httpd -y"
          
                          }

                       }
					   
					    stage ('httpd-start'){

                    steps {
   
                         sh "service httpd start"
          
                          }

                       } 
					   
					   stage ('index-dep'){

                    steps {
   
                         sh "cp -r index.html /var/www/html"
						  sh "chmod 777 /var/www/html/index.html"
						 
          
                          }

                       }
					   
              
			  }


}
