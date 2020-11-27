# Experiment 12: How to Install Docker

## Steps Performed

- Add GPG keys to verify the official docker repository.
```curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -```           
![Screenshot from 2020-11-27 02-46-43](https://user-images.githubusercontent.com/46739435/100391960-19ec3600-305b-11eb-8964-5d231bd1668d.png)

- Add docker repository.
```sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"```              
![Screenshot from 2020-11-27 02-47-39](https://user-images.githubusercontent.com/46739435/100391955-18227280-305b-11eb-8504-7291dc08afa7.png)

- Make sure you are about to install from the Docker repo.
```apt-cache policy docker-ce```                   
![Screenshot from 2020-11-24 16-39-58](https://user-images.githubusercontent.com/46739435/100391984-283a5200-305b-11eb-8789-e408b0508004.png)

- Install Docker
```sudo apt-get install -y docker-ce```                           
![Screenshot from 2020-11-24 18-02-38](https://user-images.githubusercontent.com/46739435/100391980-26708e80-305b-11eb-94c1-260be0ff96ca.png)

