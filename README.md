# ref-rt-infra
ref-rt-infra
Ubuntu Server 24.04 LTS (HVM), SSD Volume Type
```
sudo su
apt-get update
git clone https://github.com/its-a-feature/Mythic
cd Mythic/
./install_docker_ubuntu.sh
apt-get install make
make
sudo -E ./mythic-cli install github https://github.com/MythicAgents/Apollo.git
```
