pipeline 
{   
   agent {
     label 'Build-Nginix'
         }   
     stages 
    {
       stage ('Checkout') 
          {
           steps {
             node ('Build-Nginix') {
               checkout scm
                                   }
                 }
            } 
       
        stage ('NginxDeployment')
        {
           steps {
              node ('Build-Nginix')
                   {
                sh 'sudo cp /home/ubuntu/workspace/MyPipelinejob1/* /var/www/html/ '             
                   }
                 } 
        }
    }
}
