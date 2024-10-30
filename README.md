# For staging

ansible-playbook -i inventory.yml site.yml --limit staging

# For production

ansible-playbook -i inventory.yml site.yml --limit production
