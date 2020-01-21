pipeline {
    agent { label 'master'}

    parameters{
        string(name:'AWS_ACCESS_KEY', defaultValue: '', description: 'AWS_ACCESS_KEY')
        string(name:'AWS_SECRET_ACCESS_KEY', defaultValue: '', description: 'AWS_SECRET_ACCESS_KEY')
    }
    stages {
        stage('Terraform Destroy'){
            steps{
                  sh(
                      '''
                      sh 'scripts/terraform-destroy.sh'
        
                      '''  
                  )
            }

        }
        stage('Terraform plan'){
            steps{
                  sh(
                      '''
                      sh 'scripts/terraform-plan.sh'
                      '''  
                  )
            }

        }
        stage('Terraform Plan'){
            steps{
                  sh(
                      '''
                      sh 'scripts/terraform-plan.sh'
                      '''  
                  )
            }
        }
        stage('Terraform plan'){
            steps{
                  sh(
                      '''
                      sh 'scripts/terraform-plan.sh'
                      '''  
                  )
            }
        }
        stage('Terraform out'){
            steps{
                  sh(
                      '''
                      sh 'scripts/terraform-out.sh'
                      '''  
                  )
            }
        }
        stage('Inspec  install'){
            steps{
                  sh(
                      '''
                      sh 'scripts/inspec-install.sh'
                      '''  
                  )
            }
        }
        stage('Inspec test execution'){
            steps{
                  sh(
                      '''
                      sh 'scripts/inspec-test.sh'
                      '''  
                  )
            }
        }
        stage('Terra destroy'){
            steps{
                  sh(
                      '''
                      sh 'scripts/terraform-destroy.sh'
                      '''  
                  )
            }
        }
    }
}