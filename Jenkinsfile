pipeline {
	agent any
		stages {
			stage('Build') { 
				agent {
					docker {
						lable 'docker'
							image 'registry.cn-hangzhou.aliyuncs.com/eryajf/node:11.15'
					}
				}
				stages {
					stage('Build') { 
						steps {
							sh 'npm install --registry=https://registry.npm.taobao.org' 
						}
					}
				}
			}

		}

}
