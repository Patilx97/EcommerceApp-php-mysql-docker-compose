# Run PHP-MYSQL project from docker-compose

## 1. Launch EC2 instance & allow port 80
## 2. Connect to server via SSH or direct
## 3. Update package lists 
```bash
$ sudo apt-get update -y
```
## 4. Install docker-compose from script to avoid errors, create bash script for it.  
Copy script from following this [link](https://github.com/slyfox1186/script-repo/blob/main/Bash/Misc/docker-compose-multi-arch.sh) 
 
Create bash file and paste that copied script:
```bash
$ sudo nano file.sh
```    
Give permission for execute that file: 
```bash
$ sudo chmod +x file.sh
```
And run that script, it will install docker-compose:
```bash
$ sudo ./file.sh 
```
## 5. Install docker 
```bash
$ sudo apt-get install docker.io
```   
## 6. Clone the project repository
I have already created dockerfile & docker-compose file in this repository
```bash
$ git clone https://github.com/stark303test/app-ecommerce-php-mysql.git
```
## 6. Now run the docker-compose file 
```bash
   $ sudo docker-compose up -d 
```
Now, you will see your containers running. 

Just copy your instance's public IP and paste it into your browser, the project will be running.

Take a look at the Dockerfile and docker-compose file to understand how it works exactly.

