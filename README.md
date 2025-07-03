# ansible_tutorial

## bootstrap
`ansible-playbook bootstrap.yml --ask-pass --ask-become-pass -e 'ansible_user=piotr ansible_ssh_private_key_file=none'`

## komendy

```bash
ansible all -m ping
ansible all -m gather_facts
ansible all -m gather_facts --limit 192.168.1.44
ansible all -m apt -a name=tmux --become --ask-become-pass
ansible all -m apt -a "upgrade=dist" --become --ask-become-pass
ansible-playbook --ask-become-pass site.yml
ansible-playbook --list-tags site.yml
ansible-playbook --tags "db,apache" --ask-become-pass site.yml
```

## TODO
- ansible lint https://www.redhat.com/en/blog/ansible-lint
- ansible lightspeed