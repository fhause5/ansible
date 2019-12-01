# Ansible

* ssh-keygen -t rsa -f ansible_ssh
* sudo chmod 400 ansible_key
* ansible-playbook -i inv.txt playbook1.yml -e "hosts=all"
* ansible-playbook -i inv.txt playbook1_idvit.yml -e "hosts=all" --tags=test
* export ANSIBLE_SSH_PIPELINING=True
Example with env:
```
export AWS_ACCESS_KEY_ID=AKIAIOSFODNN7EXAMPLE
export AWS_SECRET_ACCESS_KEY=wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
export AWS_DEFAULT_REGION=us-west-2

```
ERRORS
```
fatal: [host2 -> 127.0.0.1]: FAILED! => {"changed": false, "module_stderr": "sudo: a password is required\n", "module_stdout": "", "msg": "MODULE FAILURE\nSee stdout/stderr for the exact error", "rc": 1}
```
* sudo -i
