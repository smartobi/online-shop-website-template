pipeline {
    agent any
    stages {
        stage('---install apache---') {
            steps {
                sh "sudo apt install apache2 -y"
                sh "sudo systemctl status apache2"
            }
        }
        stage('---install some tools---') {
            steps {
                sh "sudo apt install wget zip unzip -y"
                sh "sudo unzip file"
            }
        }
        stage('--download source webfile--') {
            steps {
                sh "sudo cp -rf html/* /var/www/html/"
               
            }
        }
        stage('--restart the apache2 server--') {
            steps {
                sh "sudo systemctl restart apache2"
            }
        }
    }
}