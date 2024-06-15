# MediaWiki-
MediaWiki  App - Terraform and Ansible Integration
Integrating Terraform infrastructure provisioning and Ansible configuration management for end-to-end automation.

Requirements
Automate the deployment of MediaWiki using steps https://www.mediawiki.org/wiki/Manual:Running_MediaWiki_on_Red_Hat_Linux#Final

Solution
This solution provisions instances using Terraform.

- Uses RHEL 8 AMI
- Create AWS key pair
- Create AWS security group
- Create EC2 instance with remote-exec and local-exec provisioner triggering Ansible
Pre-requisites
Create new ssh key or use existing ssh key which is used to connect to instance created by terraform.

By default ssh key file names and path is: ~/.ssh/id_rsa

Variables can be changed by adding variable values in terraform.tfvars.

pub_key_file: ""
prv_key_file: ""
Can change instance count. By default its 1.

instance_count: 2
Default region is us-west-2

       
