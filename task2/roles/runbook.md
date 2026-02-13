Инструкция: 
1. 
```bash
sudo mkdir -p /tmp/nginx-test        
echo "server { listen 80; }" | sudo tee /tmp/nginx-test/nginx.conf
```
2. 
```bash
 ansible-playbook -i inventory.ini deploy.yaml 
```
3. 
```bash
 cat /tmp/nginx-test/nginx.conf
```