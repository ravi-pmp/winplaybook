#Setting up the project

1. Install the collection from downloads folder

```shell
cd <root_folder_project>

cp downloads/ansible_collections/* .

ansible-galaxy collection install ansible-utils-2.2.0.tar.gz -p collections

ansible-galaxy collection install community-general-3.7.0.tar.gz -p collections
```

2. Installing the pyexel python library
Step 3: Untar the openpy excel package and their dependencies 



```shell
tar -zxvf downloads/extra_python_lib/pyexcel.tar.gz
```

Step 4: 
```shell
pip install -r pyexcel/requirements.txt --no-index --find-links pyexcel
```

Step 5:
```shell
cd /usr/local/lib64/python3.6/site-packages
find . -type d -exec chmod o+rx {} \;
find . -type f -exec chmod o+r {} \;

cd /usr/local/lib/python3.6/site-packages
find . -type d -exec chmod o+rx {} \;
find . -type f -exec chmod o+r {} \;

```
