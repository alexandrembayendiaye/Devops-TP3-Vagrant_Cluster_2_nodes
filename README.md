"# Devops-TP3-Vagrant_Cluster_2_nodes" 
1.	Création de 2 machines web et db
![a13](https://github.com/user-attachments/assets/9e9fadfe-3f6b-4736-a37f-b4a633eda043)
pour se connecter au serveur web
3.	Installer node js
a.	Taper curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash – pour ajouter le depot officiel de node js
b.	sudo apt install -y nodejs
![a14](https://github.com/user-attachments/assets/28b42ded-ac95-4177-a9c2-2bcec1a14c2a)
4.	Installer JAVA et Maven
a.	sudo apt update
b.	sudo apt install -y software-properties-common && sudo add-apt-repository ppa:openjdk-r/ppa pour ajouter le PPA à mon système
c.	sudo apt install -y openjdk-17-jdk maven
![a15](https://github.com/user-attachments/assets/a8cc2653-6dc4-46fd-8455-8de4594678da)
5.	git clone https://github.com/ngorseck/admin-app.git pour cloner le projet
6.	nano admin-app/src/main/resources/application.yml
![a16](https://github.com/user-attachments/assets/7fdf6e65-39d8-4355-afa9-f34c2b13a902)
7.	mvn clean package
8.	java -jar target/*.jar --server.port=8086
9.	Se connecter et créer la base de données
![a17](https://github.com/user-attachments/assets/4166fa1f-ea78-4e4e-b0fc-e86729b4ebb9)





