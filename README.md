```buildoutcfg

# execute playbook
ansible-playbook -i inventory.txt playbook-wv.yaml

# execute playbook and pass Jenkins build number var into Ansible playbook
ansible-playbook -i inventory.txt --extra-vars '{"build_no":"1.13"}' playbook-wv.yaml
# or
BUILD_NUMBER=1.13
ansible-playbook -i inventory.txt --extra-vars "{'build_no':$BUILD_NUMBER}" playbook-wv.yaml

# execute ansible playbook as a different user than the Ansible ssh user
ansible-playbook -i inventory.txt playbook-remote_user.yaml

```
