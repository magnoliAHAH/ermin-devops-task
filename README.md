# Порядок выполнения  
## Первые 3 пункта задания  
ansible-playbook -i inventory.ini setup-ssh.yml

## Весь 4 пункт  
ansible-playbook -i inventory.ini postgres-setup.yml

## 5 пункт задания  
ansible-playbook -i inventory.ini nginx-setup.yml

## 6 пункт задания  
ansible-playbook -i inventory.ini access-setup.yml

## 7 пункт задания  
ansible-playbook -i inventory.ini backup-setup.yml

# Особенности  
inventory файл дожен содержать следующие имена хостов  
hostA.renue 
hostB.renue  
Также ip должен указываться в параметре с названием ansible_host  

Используется Postgres 16  

Можно создать новые ключи в .ssh с именем id_rsa id_rsa.pub  

при первом запуске, если в known hosts не добавлены хосты, то запустить, ответить yes, перезапустить и ещё раз yes
