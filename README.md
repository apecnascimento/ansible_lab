# Ansible lab
This vagrant file creates a complex scenario. The scenario includes a load balance machine two servers to application and one server to the database. The idea is to create a lab that you can practice simples ansibles commands and complex deploy orchestration too.

### Create and start a lab
```sh
$ vagrant up
```

### Remove all machines
```sh
$ vagrant destroy
```

### Test machines connectivity
```sh
$ ansible mult -i hosts -m ping
```
Expeted response:
```sh
192.168.100.5 | SUCCESS => {
    "changed": false, 
    "ping": "pong"
}
192.168.100.3 | SUCCESS => {
    "changed": false, 
    "ping": "pong"
}
192.168.100.4 | SUCCESS => {
    "changed": false, 
    "ping": "pong"
}
192.168.100.6 | SUCCESS => {
    "changed": false, 
    "ping": "pong"
}
```



