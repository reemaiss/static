pipeline {
     agent any 
     stages {
       stage('Upload to AWS'){
          steps{
            withAWS(region:’US East(Ohio)’,credentials:’ststic3’) {
            s3Upload(pathStyleAccessEnabled:true, payloadSigningEnabled: true, file:’index.html’, bucket:jenkinsbucketrema)
          }
          }
       }  
     }
}