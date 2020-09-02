pipeline {
   
   agent {
     label 'Build-Nginix'
     } 
   
     stages {
       stage ('Checkout') 
          {
           steps {
             node ('Build-Nginix') {
               checkout scm
                                   }
                 }
            } 
       }
}
