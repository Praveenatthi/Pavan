piline{
    agent any
    environments{
        TOMCAT_IP = "10.10.10.10"
        TOMACT_USER = "EC2-USER"
    }
    stages{
        stage(cloneing stage){
            steps{
                echo " cloneing sucessfull"
            }
        }
    }
    stages{
        stage(build stage){
            steps{
                echo"build is sucessfull"
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
