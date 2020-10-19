DOCKER INSTALLATION

  Method-1:  using a Script :
  ========================
               $ curl -fsSL https://get.docker.com -o get-docker.sh
               $ sudo sh get-docker.sh 
               $ docker -version

                                                    [OR]

   Method-2:  using a Commands:
   ==========================
Step-1:  to Setup a Repository:
--------------------------------------------

$ sudo apt-get update

$ sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg-agent \
    software-properties-common


$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

$ sudo apt-key fingerprint 0EBFCD88

$ sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"

Step-2:  to Install Docker Engine :
----------------------------------------------
 $ sudo apt-get update
 $ sudo apt-get install docker-ce docker-ce-cli containerd.io

$ apt-cache madison docker-ce

   Select a required version of Docker Engine :  5:19.03.13~3-0~ubuntu-bionic

Syntax:
   $ sudo apt-get install docker-ce=<VERSION_STRING> docker-ce-

cli=<VERSION_STRING> containerd.io

Ex: 
   $ sudo apt-get install docker-ce=5:19.03.13~3-0~ubuntu-bionic docker-ce-

cli=5:19.03.13~3-0~ubuntu-bionic containerd.io


 $ docker --version
Docker version 19.03.13, build 4484c46d9d

$ sudo docker run hello-world

Hello from Docker!
