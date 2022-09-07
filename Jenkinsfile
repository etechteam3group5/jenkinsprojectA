pipeline {
	agent any
		stages{
			stage('1-Clone Repository - Maxwell Chinedu'){
				steps{
					checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-id', url: 'https://github.com/etechteam3group5/jenkinsprojectA.git']]])
				}
			}
			stage('2-User Check - Christiana Gabriels'){
				steps{
					sh 'whoami'
					sh 'date'
				}
			}
			stage('3- directory check -Waisu Lawal'){
				steps{
					sh "pwd"
					sh "ls"
				}
			}
			stage('4-Process check - Tunde Onowofokan'){
				steps{
					sh 'ps -ef'
					sh 'sudo systemctl status jenkins'
				}
			}
			stage('5-Sshd check - Chima Ikemelu'){
				steps{
					sh 'cat /etc/ssh/sshd_config'
					sh 'sudo systemctl status sshd'
				}
			}
			stage('6-Volume check -Gregory Rotilli'){
				steps{
					sh 'lsblk'
					sh 'df -h'
				}
			}
			stage('7-Network Check - Chizoba'){
				steps{
					sh 'ip a'
					sh 'netstat'
				}
			}
			stage('8-Memory Check - Valentine Erondu'){
				steps{
					sh 'free -g'
					sh 'free -m'
					
				}
			}
		}
	}