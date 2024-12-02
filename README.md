# 軟體開發
## [2024-12-02 雁行計畫 微處理器系統](https://www.canva.com/design/DAGXik4geYs/agOZm04OFkar4gWpl0Ypbg/view?utm_content=DAGXik4geYs&utm_campaign=designshare&utm_medium=link&utm_source=editor)
### Google Colab 實際操作(簡報:p35-p38)
```
無 CLI 指令操作
```
### 原生系統下的版本控制實際操作(簡報:p39-p43)
```bash
git config --global user.name "Your Name"
git config --global user.email <Your Email>
```
### 原生系統下運行虛擬化技術的軟體實際操作(簡報:p47-p50)
```
無 CLI 指令操作
```
### Debian/Ubuntu 安裝 docker.io (簡報:p51-p57)
#### 更新與升級套件，並安裝 docker.io
```bash
sudo apt-get update && sudo apt-get upgrade -y
sudo apt-get install docker.io -y
sudo systemctl enable docker
sudo usermod -aG docker $USER
sudo systemctl restart docker
sudo reboot
```
#### 下載 ubuntu 24.04 映像檔
```bash
docker pull ubuntu:24.04
```
#### 建立 ubuntu 24.04 容器
```bash
docker run -it -d --name ubuntu-24.04-container ubuntu:24.04
```
#### 進入容器
```bash
docker exec -it ubuntu-24.04-container /bin/bash
```
#### 容器內部安裝 neofetch 並顯示系統資訊
```bash
apt update && apt install -y neofetch
neofetch
```