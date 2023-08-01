pipeline {
     agent any
     stages {
	   stage ('copy-index') {
	      steps {
		     sh 'cp -r index.html /var/www/html/'
		  }
	   }
	 stage ('copy-dev') {
	    steps {
		  sh 'cp -r dev.html /var/www/html/'
		}
	 }
	stage ('cy-qa') {
	  steps {op
	  sh 'cp -r qa.html /var/www/html/'
	  }
	} 
	stage ('restart-apache') {
	  steps {
	    sh 'service httpd restart'
	  }
	}
	 }	 
}
