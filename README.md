## create server
```
ansible -i hosts all --list-hosts | tail -n +2 | xargs openstack server create --image centos-7.2 --flavor m1.large --flavor --key-name niko
```

## setup
```
ansible-playbook -i hosts setup.yml
```

## docker
```
ansible-playbook -i hosts docker.yml
```

## consul
```
ansible-playbook -i hosts consul.yml
```

## nomad
```
ansible-playbook -i hosts nomad.yml
```
