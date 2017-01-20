## create server
```
ansible -i hosts all --list-hosts | tail -n +2 | xargs openstack server create --image centos-7.2 --flavor m1.large --flavor --key-name niko
```

## setup server
```
ansible-playbook -i hosts setup.yml
```

## setup docker
```
ansible-playbook -i hosts docker.yml
```

## setup consul
```
ansible-playbook -i hosts consul.yml
```

## setup nomad
```
ansible-playbook -i hosts nomad.yml
```
