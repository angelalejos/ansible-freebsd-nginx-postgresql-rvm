# Ansible FreeBSD Nginx Postgresql RVM

Installs Nginx Postgresql RVM for a Rails app.

### Workstation setup
Installs RVM role for Ansible
```sh
$ ansible-galaxy install rvm_io.rvm1-ruby
```

### Remote server setup
FreeBSD does not come with python. Install it with

```sh
# pkg install python
```

### Setup
Edit the vars in the ```hosts``` file as you need.
### Launch
```sh
$ ansible-playbook site.yml -i hosts -K
```
Notes
----
I am not following Ansible's best practices regarding directory structure:

http://docs.ansible.com/ansible/playbooks_best_practices.html#directory-layout
