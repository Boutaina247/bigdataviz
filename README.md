# Topic 

# How to use 

(Verify you have docker and wsl2 on your computer)

* Clone the project on your computer
Execute docker compose in the directory where you have put docker compose file

-> docker-compose up 

if it crash, do another test

* Connexion machnine
All machines must have good communication between them, we must test it with ping from machine to another machine

Enter into a machine

-> docker exec -it namenode

test ping from namenode to spark-master

-> ping spark-master

* Do update upgrade 

-> apt update

-> apt upgrade

-> apt-get python3 

* Copy file from locale to namenode hadoop machine 

->  docker cp "C:\MASTER\Master1\Semestre1\Big Data & DataViz\test_project\Données\Donnees\objets-trouves-restitution.csv" namenode:/root/

->  docker cp "C:\MASTER\Master1\Semestre1\Big Data & DataViz\test_project\Données\Donnees\regularite-mensuelle-intercites.csv" namenode:/root/


* verify if files are copied 

* move files to hadoop

Create directory on hadoop -> hdfs dfs -mkdir /data

-> docker exec -it namenode bash 

-> hdfs dfs -put <file path on namenode> <file on hadoop>
-> hdfs dfs -put "*.csv" /data






# Authors 

### Lydia 
### Boutaina 
### Shadrack
### Kafia
