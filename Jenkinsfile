pipeline {

    environment {
        IMAGE_NAME = "lab9"
        USERNAME = "tnganthuy"
        CONTAINER_NAME = "staticdiranewebsite"
        EC2_PRODUCTION_HOST = "54.165.241.178"
		    EC2_STAGING_HOST = "3.86.184.241"
    }

    agent none

    stages{

       stage ('Build Image'){
           agent any
           steps {
               script{
                   sh 'docker build -t $USERNAME/$IMAGE_NAME:$BUILD_TAG .'
               }
           }
       }
    }
}
