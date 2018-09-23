# Flask-App-Ansible
To deploy a sample Flask application on an Amazon EC2 AMI 2.

### Edit the hosts file with the IP and Key before usage:

Ec2IP = IP of your Ec2.
KeyPath = private key path.

[webserver]
Ec2IP  ansible_port=22  ansible_user='ec2-user'  ansible_ssh_private_key_file='KeyPath'

## Usage:
ansible-playbook -i hosts Flask.yml
