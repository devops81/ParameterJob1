pipeline {
    agent any
    parameters { choice(name: 'ENV', choices: ['Dev', 'Qa', 'Prod'], description: '') }
    stages {
        stage("PARAM 1") {
            steps {
                build job: 'job_2_pipeline', parameters: [string(name: 'ENV', value: "${params.ENV}")]
            }
        }
    }
}
