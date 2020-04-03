```buildoutcfg

# execute playbook
ansible-playbook -i inventory.txt playbook-wv.yaml

# execute playbook and pass Jenkins build number var into Ansible playbook
ansible-playbook -i inventory.txt --extra-vars '{"build_no":"1.13"}' playbook-wv.yaml



```
