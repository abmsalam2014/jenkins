pipeline {
    agent { label "linux-agent" }

    // parameters {
    //     string(name: 'NAME', defaultValue: '', description: 'What is your Full Name?')
    //     choice(name: "Branch", choices: "main\ndev", description: "Select Branch")
    // }

    // pre{

    // }

    stages{

        stage("Build") {
          when {
            anyOf {
                branch 'main'
            }
          }
          steps {
              cleanWs()
              echo "In Stage Build"
            }
        }

        stage("Deploy") {
            steps {
              echo "In Stage Deploy"

            }
        }
    }

    post {
        always {
            cleanWs()
        }

    }



}