pipeline{
    agent any

    tools{
        maven "jenkins-maven"
    }

    stages{

        stage("Test"){
            steps{
               echo "Testing the app !"
            }
        }
        
        stage("Build"){
            when {
                expression {
                    BRANCH_NAME == "main"
                }
            }
            steps{
               echo "Building the app !"
            }
        }
         stage("Deploy"){
              when {
                expression {
                    BRANCH_NAME == "main"
                }
            }
            steps{
               echo "Building the app !"
            }
        }
    }
}
