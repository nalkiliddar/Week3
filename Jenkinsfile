pipeline {
    agent none // Master
    stages {
        stage('Run 4 Pipelines Concurrently') {
            parallel {
                stage('Pipeline 1') {
                    agent { label 'docker-agent' }
                    stages {
                        stage('Build') {
                            steps {
                                sleep 300
                                echo 'this is pipeline 1'
                            }
                        }
                    }
                }
                stage('Pipeline 2') {
                    agent { label 'docker-agent' }
                    stages {
                        stage('Build') {
                            steps {
                                sleep 300
                                echo 'this is pipeline 2'
                            }
                        }
                    }
                }
                stage('Pipeline 3') {
                    agent { label 'docker-agent' }
                    stages {
                        stage('Build') {
                            steps {
                                sleep 300
                                echo 'this is pipeline 3'
                            }
                        }
                    }
                }
                stage('Pipeline 4') {
                    agent { label 'docker-agent' }
                    stages {
                        stage('Build') {
                            steps {
                                sleep 300
                                echo 'this is pipeline 4'
                            }
                        }
                    }
                }
            }
        }

        stage("Build") {
            
            steps {
                    echo 'this is the main branch'
            }
        }
        
    }
}
