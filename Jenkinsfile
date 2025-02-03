pipeline {
    agent {
    	node{
	  label "linux && java11"
	}
    }
    stages {
        stage("Build") {
            steps {
                echo ("Hello Build")
            }
        }

        stage("Test") {
            steps {
                echo ("Hello Test")
            }
        }

        stage("Deploy") {
            steps {
                echo ("Hello Deploy")
            }
        }
    }
    post {
        always {
            echo " I will always say Hello again!"
        }
        success {
            echo "yeay, Succes!!!"
        }
        failure { 
            echo "Oh no, Failure!!"
        }
        cleanup {
            echo "Dont care succes or error"
        }
    }
}
