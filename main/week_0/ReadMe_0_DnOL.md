# OpenLane Installation Steps

### Docker Installation

    $ sudo apt-get update 
    $ sudo apt-get upgrade
    $ sudo apt install -y build-essential python3 python3-venv python3-pip make git
    $ sudo apt install apt-transport-https ca-certificates curl software-properties-common curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
    $ echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null 
    $ sudo apt update
    $ sudo apt install docker-ce docker-ce-cli containerd.io 
    $ sudo docker run hello-world
    $ sudo groupadd docker
    $ sudo usermod -aG docker $USER sudo reboot

### After reboot

    $ docker run hello-world

## Check dependencies

    $ git --version 
    $ docker --version 
    $ python3 --version
    $ python3 -m pip --version 
    $ make --version
    $ python3 -m venv -h

## Below steps installs PDKs and Tools
    $ cd $HOME
    $ git clone https://github.com/The-OpenROAD-Project/OpenLane cd OpenLane
    $ make make test



## 6. Docker

### Docker Installation Steps

### Verification - Docker Installation 
![Docker](https://github.com/poonamkasturi/RTLtoGDS_RISC_V_VSD_IITGN/blob/main/main/week_0/assets/Docker.png)
_________________________________________________________________________________________________________________________
## 7. Versions of tools installed

### Versions of the tools installed
![Versions_Tools](https://github.com/poonamkasturi/RTLtoGDS_RISC_V_VSD_IITGN/blob/main/main/week_0/assets/versions.png)
