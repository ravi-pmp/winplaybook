
#User Operation via excel file

##No entries in the excel file.(Negative Scenario)
```shell

ansible-playbook -i inventory  user_operation.yml -e \
'{
  "config_type": "users",
  "excel_file_name": "LocalUserOperation.xlsx"
}'
```

##Single entry in the excel file but server name is empty.(Negative Scenario)
```shell

ansible-playbook -i inventory  user_operation.yml -e \
'{
  "config_type": "users",
  "excel_file_name": "LocalUserOperation_EmptyServerColumn.xlsx"
}'
```
##Single entry in the excel file - Positive scenario

```shell
ansible-playbook -i inventory  user_operation.yml -e \
'{
  "config_type": "users",
  "excel_file_name": "LocalUserOperation_Positive.xlsx"
}'
```
