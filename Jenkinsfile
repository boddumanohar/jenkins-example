pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven {
                    sh 'mvn clean compile'
                }

                script {
                    sh ('ls -al')
                    sh ('ls -al target/')
                }
            }
        }

        // stage ('Testing Stage') {

        //     steps {
        //         withMaven {
        //             sh 'mvn test'
        //         }
        //     }
        // }

        // stage ('Deployment Stage') {
        //     steps {
        //         withMaven {
        //             sh 'mvn deploy'
        //         }
        //     }
        // }
    }
}
