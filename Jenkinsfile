pipeline {​
​
    agent any ​
​
    stages {​
​
        stage('Git') { ​
​
            steps {​
​
                git url:'https://github.com/GitRep2018/BOOKLENDING_UI.git'
​
            }​
​
        }​
​
        ​
          stage('Build') { ​
​
            steps {​
​
                sh '''​
​
                npm install​
​
                npm run build​
​
            '''​

            }​
​
        }​
  stage('Deploy') { ​

            steps {
		sh '''    
                cd /var/lib/jenkins/workspace/BOOKLENDING_UI_PIPELINE/dist​
​
                chmod -R 777 BookLendSystem​
​
                cp -rf BookLendSystem /opt/apache-tomcat-9.0.26/webapps/
            '''

            }

        }
