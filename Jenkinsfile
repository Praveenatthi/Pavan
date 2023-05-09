piline{
    agent any
    stages{
        stage(cloneing stage){
            steps{
                echo " git clone "https://github.com/Praveenatthi/Pavan.git"
            }
        }
    }
    stages{
        stage(build stage){
            steps{
                "sh mvn package"
            }
        }
    }
    stages{
        stage(deployed stage){
            stages(deployed stage){
                echo "usein tomcat ip going to deployed ${env.TOMCAT-IP}" user ${env.TOMCAT_USER}
            }
        }
    }
    post{
        sucess{
            echo " email send to internal team"
        }
        false{
            echo " email sent to developer team"
        }
    }
}
