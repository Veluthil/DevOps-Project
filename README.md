# DevOps Project - Learning Technologies

![Vagrant](https://img.shields.io/badge/vagrant-%231563FF.svg?style=for-the-badge&logo=vagrant&logoColor=white)
![Shell Script](https://img.shields.io/badge/shell_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Cent OS](https://img.shields.io/badge/cent%20os-002260?style=for-the-badge&logo=centos&logoColor=F0F0F0)
![RabbitMQ](https://img.shields.io/badge/Rabbitmq-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
![Apache Tomcat](https://img.shields.io/badge/apache%20tomcat-%23F8DC75.svg?style=for-the-badge&logo=apache-tomcat&logoColor=black)
![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)

This repository contains a Vagrant-based DevOps project designed to help me learn various technologies. Currently, the project consists of multiple virtual machines (VMs) set up using Vagrant and Oracle VirtualBox. Each VM is provisioned with shell scripts to install and configure specific software. Additionally, there is a Java application integrated with a MySQL database.

### Vagrantfile

The `Vagrantfile` in the vagrant/Automated_provisioning_WinMacIntel directory is the configuration file for defining and managing the VMs. It sets up the following VMs:

1. **DB VM (`db01`)**: This VM runs CentOS Stream 9 and contains a MySQL database.
2. **Memcache VM (`mc01`)**: This VM runs CentOS Stream 9 and includes a Memcache server.
3. **RabbitMQ VM (`rmq01`)**: This VM runs CentOS Stream 9 and runs a RabbitMQ messaging server.
4. **Tomcat VM (`app01`)**: This VM runs CentOS Stream 9 and deploys a Java application using Tomcat.
5. **Nginx VM (`web01`)**: This VM runs Ubuntu Jammy 64 and hosts an Nginx web server.

### Shell Scripts

Each VM is provisioned using shell scripts to install and configure the required software:

- `mysql.sh`: Installs and configures MySQL on the `db01` VM.
- `memcache.sh`: Installs and configures Memcache on the `mc01` VM.
- `rabbitmq.sh`: Installs and configures RabbitMQ on the `rmq01` VM.
- `tomcat.sh`: Installs and configures Tomcat on the `app01` CentOS VM.
- `tomcat_ubuntu.sh`: Installs and configures Tomcat on the Ubuntu VM.
- `nginx.sh`: Installs and configures Nginx on the `web01` VM.

### App Structure

Java application is in the src/main/java directory, MySQL data is in the src/main/resources/db_backup.sql file.

### Disclaimer

Please note that this project is for educational purposes only. It's not intended for production use. 

### Acknowledgments

This project has been created thanks to the knowledge gained from the "Decoding DevOps" course by Imran Teli
