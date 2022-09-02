pipeline {
	agent any
		stages{
			stage('1-Clone the Repository - Maxwell Chinedu'){
				steps{
					checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-id', url: 'https://github.com/etechteam3group5/jenkinsprojectA.git']]])
				}
			}
			stage('2-Greetings'){
				steps{
					echo "We are Team 3 Group 5"
				}
			}
			stage('3-User check - Christiana Gabriels'){
				steps{
					logname
					whoami
				}
			}
			stage('4-startup check - Waisu Lawal'){
				steps{
					date
					pwd
					ls
				}
			}
			stage('5-Process Monitor - Tunde Onafowokan'){
				steps{
					ps -ef
					sudo systemctl status jenkins
				}
			}
			stage('6-Ssh daemon Check - Chima Ikemelu'){
				steps{
					cat /etc/ssh/sshd_config
					sudo systemctl status sshd
				}
			}
			stage('7- Disk usage check - Gregory Rotilli'){
				steps{
					du -h
					df -h
				}
			}
			stage('8-Cpu check - Chizoba'){
				steps{
					top
					lscpu
				}
			}
			stage('9- memory check - Valentine Erondu'){
				steps{
					free -g
					free -m
					
				}
			}
		}
	}
