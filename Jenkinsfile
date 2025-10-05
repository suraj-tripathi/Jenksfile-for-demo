@Library('jenkins-class-lib@main') _
import org.opstree.Utils
pipeline {
    agent any

    stages {
        stage('Initialization') {
            steps {
                echo "Pipeline execution started in the application repository."
            }
        }
        
        stage('Shared Library Execution') {
            steps {
                script {
                    sayHello('Adeel')

                    def u = new Utils(this)
                    u.runSampleMethod("Hello world !")    
                }
            }
        }
        stage('Completion') {
          steps {
            echo "Shared library functions executed successfully!"
          }
       }
    }
}
          
