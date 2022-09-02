pipeline {
	agent any
		stages{
			stage('1-Clone Repository - Maxwell Chinedu'){
				steps{
					checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-id', url: 'https://github.com/etechteam3group5/jenkinsprojectA.git']]])
				}
			}
			stage('2-Greetings'){
				steps{
					echo "We are Team3 Group5"
				}
			}
			stage('3-User Check - Christiana Gabriels'){
				steps{
					sh 'whoami'
					sh 'date'
				}
			}
			stage('4- directory check -Waisu Lawal'){
				steps{
					sh "pwd"
					sh "ls"
				}
			}
			stage('5-Process check - Tunde Onowofokan'){
				steps{
					sh 'ps -ef'
					sh 'sudo systemctl status jenkins'
				}
			}
			stage('6-Ssh daemon check - Chima Ikemelu'){
				steps{
					sh 'cat /etc/ssh/sshd_config'
					sh 'sudo systemctl status sshd'
				}
			}
			stage('7-Volume check -Gregory Rotilli'){
				steps{
					sh 'lsblk'
					sh 'df -h'
				}
			}
			stage('8-Network Check - Chizoba'){
				steps{
					sh 'ip a'
					sh 'netstat'
				}
			}
			stage('9-Memory Check - Valentine Erondu'){
				steps{
					sh 'free -g'
					sh 'free -m'
					
				}
			}
		}
	}