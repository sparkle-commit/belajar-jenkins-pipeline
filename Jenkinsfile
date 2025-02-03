pipeline {
    agent {
    	node{
	  label "linux && java11"
	}
    }
    stages {
        stage('Helloo') {
            steps {
                echo 'Hello World'
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
