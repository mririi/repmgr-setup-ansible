# Run
* run the standby playbook
```
ansible-playbook -i hosts repmgr_setup_master.yml -K
```

* run the standby playbook
```
ansible-playbook -i hosts repmgr_setup_standby.yml -K
```
* check that all is working on the second standby node
```
sudo -u postgres repmgr -f /etc/repmgr/12/repmgr.conf cluster show
```
