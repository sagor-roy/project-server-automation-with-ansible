### LAMP Project for Flexible and Efficient Server Deployment

This project automates the deployment of the LAMP (Linux, Apache, MySQL, PHP) stack on servers, aimed at improving flexibility and reducing time consumption. It includes configurations for setting up Apache, MySQL, and PHP, along with essential project files and an environment setup for Laravel applications. The automation process enables faster and more reliable deployments, allowing for scalable server management.


## Key in secrets.yml file
```
ec2_access_key: "xxxxxxx"
ec2_secret_key: "xxxxxxx"
mysql_root_password: "xxxxxxx"

```

## CMD for Playbook Run
```
ansible-playbook aws.yml --ask-vault-pass
ansible-playbook -i inventory/hosts deploy.yml --ask-vault-pass
ansible-vault encrypt group_vars/all/secrets.yml

```
