node{
stage('Clone') {
git 'https://github.com/david-ipssi2021/app-salaire.git'
}
stage('Ansible') {
ansiblePlaybook (
colorized: true,
become: true,
playbook: 'playbook.yml',
inventory: 'hosts.yml'
disableHostKeyChecking: false
)
}
}
