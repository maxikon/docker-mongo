# Mongo in Docker via Ansible

To install on remote host please change:
- **inventory** file
- vault **passwd** file
- **keys** in folder keys (I understand that publishing keys is not good :) )

Password is **qwerty123456** for vault, remote user, mongo root

How to run:
```sh
$ ansible-playbook -i inventory --ask-vault-pass --extra-vars '@passwd.yml' install.yml
```

