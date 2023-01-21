# Workshop for ansible in ec2 aws

# Activate the python ansible
conda activate ansible


copy the key pair to ec2 instance using scp
scp -i '/key/key.pair' file.pem ec2-user@13.214.121.209:/home/ec2-user/file.pem


```
ssh-agent bash
```

```
cp file.pem ~/.ssh/
```



```
ssh-add ~/.ssh/file.pem
```



```
Editor
ansible-target-1 ansible_host=13.214.121.209 ansible_connection=ssh ansible_user=ec2-user

ansible-target-2 ansible_host=13.214.145.108 ansible_connection=ssh ansible_user=ec2-user


```

## Run
```
ansible ansible-target-1 -m ping -i inventory
```



