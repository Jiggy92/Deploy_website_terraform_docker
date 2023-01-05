# In this project use terraform to install and run a docker image for nginx:

Create an AWS EC2 instance/ Ubuntu
Install terraform in EC2 intsance with below links:-
**sudo apt-get update && sudo apt-get install -y gnupg software-properties-common**

Install Hashicorp key GPG:-
**wget -O- https://apt.releases.hashicorp.com/gpg | \
  gpg --dearmor | \sudo tee /usr/share/keyrings/hashicorp-archive-keyring.gpg

Verify the key fingerprint:-
**gpg --no-default-keyring \--keyring /usr/share/keyrings/hashicorp-archive-keyring.gpg \--fingerprint

Adding Hashicorp repo in your system:-
**echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] \https://apt.releases.hashicorp.com $(lsb_release -cs) main" | \
  sudo tee /etc/apt/sources.list.d/hashicorp.list

Download package info from hashicorp:-
**sudo apt update**

Install Terraform:-
**sudo apt-get install terraform**
