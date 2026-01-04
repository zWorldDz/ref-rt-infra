# ref-rt-infra
ref-rt-infra\
Ubuntu Server 24.04 LTS (HVM), SSD Volume Type\
Mythic: v3.4.19
UI: v0.3.90\
```
sudo su
apt-get update
git clone https://github.com/its-a-feature/Mythic
cd Mythic/
./install_docker_ubuntu.sh
apt-get install make
make
sudo -E ./mythic-cli install github https://github.com/MythicAgents/Apollo.git
sudo ./mythic-cli install github https://github.com/MythicC2Profiles/http

cat Mythic/.env | grep -i MYTHIC_ADMIN_PASSWORD
ssh -L 7443:127.0.0.1:7443 ubuntu@<IP> -i key.pem
```
