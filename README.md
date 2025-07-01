# ansible_tutorial

## komendy

```bash
ansible all -m gather_facts
ansible all -m gather_facts --limit 192.168.1.44
ansible all -m apt -a name=tmux --become --ask-become-pass
ansible all -m apt -a "upgrade=dist" --become --ask-become-pass
```