# VTS-IPCamera





## 1.RaspberryPi 초기세팅하기

라즈베리파이에 OS를 심고 아래 절차를 진행한다.



```
sudo apt-get update
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
sudo usermod -aG docker ${USER}
sudo reboot


docker version
docker info
docker run hello-world
sudo systemctl enable docker
sudo apt install docker-compose

docker-compose --version

```

