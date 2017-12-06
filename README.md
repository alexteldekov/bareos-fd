# bareos-fd
Bareos filedaemon installation:
```
$ cat <EOF >bareos-fd.yml
- hosts: clients
  become: true
  roles:
    - bareos-fd
EOF
$ ansible-playbook bareos-fd.yml -l hostname
```
