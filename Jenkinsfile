pipeline{

   agent any
   
    tools{
            jdk 'myjava'
            maven 'mymaven'

     }
      
   stages{

       stage('gitcheckout'){
         steps{
                     git 'https://github.com/kliakos/sparkjava-war-example.git'
         }
}


     stage('package'){
         steps{
                    sh 'mvn package'
        }

    }
        stage('deploy'){
             steps{
                sh '/opt/deploy.sh'
}
} 
          
}








}
