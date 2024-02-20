# DevOps Prerequisites 

## Introduction
source : [DevOps Prerequisites Course - Getting started with DevOps - FREE](https://youtu.be/Wvf0mBNGjXY)

Curiculum : 
1. Linux Basics
2. Setup Lab Environment
3. VirtualBox
4. Vagrant
5. Linux Networking
6. JSON/YAML

## Cloud Research
### Linux Basics
- Bourne Shell (Sh Shell)
- C Shell (csh or tcsh)
- Z Shell (zsh)
- Bourne again Shell (bash)

### Basic Command 
- echo : print to screen
- ls : list files & folders
- cd : change directory
- pwd : present working directory
- mkdir : make directory
- multiple command : cd /var; mkdir www; pwd;
- mkdir -p /test/test1 : membuat directory beserta parent directorinya
- rmdir -rf : remove directory beserta 
- cp -r directory /tmp/new_directory : copy directory beserta isinya ke new_directory
- touch : create a new file
- echo “test” > file.txt : add contents to file
- cat file.txt : view contents of file
- cp file.txt copy_file.txt : copy files
- mv : move or rename file
- rm : remove file

akses this course : https://labs.kodekloud.com/ 

> sudo : /etc/sudoers -> user yang mempunyai hak administratif setara root
> check OS version : ls /etc/*release*

### download files : 
- curl http://link-file.com/nama-file.txt -O
- wget http://link-file.com/nama-file.txt -O new-nama-file.txt

### RPM (RedHat Package Manager) : 
- rpm -i telnet.rpm → install package
- rpm -e telnet.rpm → un-install package
- rpm -q telnet.rpm → query package
- yum install → install package

### Service :
- service httpd start & systemctl start httpd : restart httpd service
- systemctl stop : stop service
- systemctl status : check service status
- systemctl enable : configure service to start ketika di start
- systemctl disable : configure service to not start ketika di start

### vi editor :
first time akan langsung ke command mode : dimana kita bisa copy,rm satu baris atau kata namun tidak bisa menulis untuk menulis kita harus masuk ke insert mode dengan click i. agar kembali ke command mode gunakan esc.

### dicommand mode kita memiliki beberapa perintah : 
![image](https://github.com/tiaradwim1306/100DaysOfDevops/assets/120786669/de9de078-6fee-493b-8909-7fe7a7e6b889)

![image](https://github.com/tiaradwim1306/100DaysOfDevops/assets/120786669/3cab7fbc-9cdf-4dfa-8d74-fc036b7c0fac)

> download image virtualbox instant : https://www.osboxes.org/virtualbox-images/ 

![image](https://github.com/tiaradwim1306/100DaysOfDevops/assets/120786669/d7e72a26-8724-4ef1-b570-f6cc69c223f0)

![image](https://github.com/tiaradwim1306/100DaysOfDevops/assets/120786669/8232911f-8bba-42ee-a16a-7fdf29914624)

### Vagrant
Vagrant provides the framework and configuration format to create and manage complete portable development environments. These development environments can live on your computer or in the cloud, and are portable between Windows, Mac OS X, and Linux.

A 'Vagrantfile' has been placed in this directory. You are now ready to vagrant up your first virtual environment! Please read the comments in the Vagrantfile as well as documentation on 'vagrantup.com' for more information on using Vagrant.

#### Vagrantfile : 
![image](https://github.com/tiaradwim1306/100DaysOfDevops/assets/120786669/a5a08064-7913-423f-991d-bd2c6666a240)

> vagran support : Virtualbox, VMWare, Hyper-V, docker and custom

download vagrant di linux/ubuntu : https://developer.hashicorp.com/vagrant/install 
```
wget -O- https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update && sudo apt install vagrant
sudo apt install vagrant
```

command : https://app.vagrantup.com/centos/boxes/7 
- vagrant init centos/7 
- vagrant up

![image](https://github.com/tiaradwim1306/100DaysOfDevops/assets/120786669/4c9ede9a-3594-49ec-8a38-448a099c8620)

![image](https://github.com/tiaradwim1306/100DaysOfDevops/assets/120786669/6e779768-060b-455d-8f61-c1f49573ddeb)

namun hal ini sangat menyusahkan jika kita harus menglist semua domain, untuk itu kita mmebutuhkan 1 server utama yang digunakan untuk setting domain/DNS, example : DNS google adalah server yang dimiliki google yang manage DNS diseluruh dunia.

![image](https://github.com/tiaradwim1306/100DaysOfDevops/assets/120786669/16afaa8b-2719-4c01-a006-41fe9f72714a)

sehingga kita cukup menambahkan ip di file resolv yang kita gunakan untuk jalan mengakses domain” tersebut

### Domain Names
- .com → for commercial
- .net → for network
- .edu → for educational organizations
- .org → non profit organizations

![image](https://github.com/tiaradwim1306/100DaysOfDevops/assets/120786669/37c5ac3b-ff2a-4634-a911-0caa6bc1fb1b)

![image](https://github.com/tiaradwim1306/100DaysOfDevops/assets/120786669/f2398a24-90c6-43c5-b3e2-01441f9a9e76)

## Social Proof
[Twitter](https://twitter.com/tiaradwim1306/status/1759853098863124701)


