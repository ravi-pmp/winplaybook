## Service Start operation
```shell
ansible-playbook -i inventory  services_operation.yml -e \
'{
  "server_names": "192.168.176.2,1.1.1.1",
  "operation":"start",
  "services": 
  [
    "sdf",
    "WSearch"
  ]
}'
```

## Service Stop operation
```shell
ansible-playbook -i inventory  services_operation.yml -e \
'{
"server_names": "192.168.176.2",
  "operation":"stop",
  "services": 
  [
    "sdf",
    "WSearch"
  ]
}'
```

## Service restart operation
```shell
ansible-playbook -i inventory  services_operation.yml -e \
'{
"server_names": "192.168.176.2",
  "operation":"restart",
  "services": 
  [
    "sdf",
    "WSearch"
  ]
}'
```