## db-[99:101]-node.example.copeline {

    agent any 

    stages {

        stage('clone and clean') { 

            steps {

                sh "git clone https://github.com/nehasonakul777/my-app.git" 

                sh "mvn clean -f my-app"

            }

        }

        stage('Test') { 

            steps {

                sh "mvn test -f my-app" 

            }

        }

        stage('Deploy') { 

            steps {

                sh "mvn package -f my-app" 

            }

        }

    }

}
