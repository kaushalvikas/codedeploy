# Ram Hemareddy AWS CICD Pipeline Code Deployment to AWS EC2 Instance


<b>User Data for Dependencies installations for ubuntu Linux 2:-</b>

#!/bin/bash<br />
sudo apt update && sudo apt -y upgrade<br />
sudo apt -y install ruby-full<br />
sudo apt -y install wget<br />
cd /home/ubuntu<br />
wget https://aws-codedeploy-ap-south-1.s3.ap-south-1.amazonaws.com/latest/install<br />
sudo ./install auto<br />
sudo apt -y install python3-pip<br />
pip3 install --user awscli<br />
echo 'export PATH=$PATH:~/.local/bin' >> ~/.bashrc<br />
source ~/.bashrc<br />
