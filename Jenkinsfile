pipeline {
    agent any

    stages {      
        stage ("terraform init") {
            steps {
                sh ('terraform init --upgrade') 
            }
        }
        
        stage ("terraform Action") {
            steps {
                echo "Terraform action is --> ${action}"
                sh ('terraform ${action} --auto-approve') 
           }
        }
    }
}
