# ansible-k8s-single-master-cluster
create k8s-single-master-cluster by ansible

# How to use it ?
## Edit hosts
In the beginning, you have to change the IP address
```
[k8s_master]
192.168.56.31

[k8s_node]
192.168.56.41
192.168.56.42
192.168.56.43
```

## Edit group_vars/all
- ansible_ssh_private_key_file: specific the path of ssh private key
```
ansible_ssh_private_key_file=/home/example/.ssh/example.pem
  
#ansible_python_interpreter: /usr/bin/python3

#ansible_connection: ssh

#ansible_ssh_user: example

#ansible_ssh_pass: example

#ansible_sudo_pass: example
```

