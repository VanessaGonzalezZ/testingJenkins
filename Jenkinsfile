pipeline {
    agent { label 'principal'}

        stages {
            stage ('install') {
                steps {
                    dir("build_node"){
                      sh "npm install"
                    } 
                }
            }
            stage ('test') {
                steps {
                  dir("build_node"){
                        sh "npm test"
                  }
                }
            }
             
        }
}
