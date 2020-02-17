node {  
  stage('Git-Checkout') {
   git 'https://github.com/smbbasha/ansible.git'
  }
 
  def project_ansible=""
dir(project_ansible) {
   stage('ansible-deploy') {
   sh 'ansible-playbook  --key=/root/.ssh/mansoor.pem  web-playbook.yaml -u ubuntu -v'
  }
  }
}
