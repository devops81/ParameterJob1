pipeline {
    agent {
                label 'LinuxAgent'
        }
        
    parameters { choice(name: 'ENV', choices: ['Dev', 'Qa', 'Prod'], description: '') }
    stages {
        stage("PARAM 1") {
            steps {
                build job: 'ParameterJob1', parameters: [string(name: 'ENV', value: "${params.ENV}")]
            }
        }
    }
}
