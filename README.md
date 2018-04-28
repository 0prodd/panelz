#!/bin/bash
echo "Removing Old Theme"
rm -rf /home/vps/public_html/asset
rm -rf /home/vps/public_html/view
rm -rf /home/vps/public_html/tmp/*
echo "Installing NoypiSSH Theme"
cd ~
mkdir M4rshall
cd M4rshall
rm -rf *
wget https://www.datafilehost.com/d/c12226e5 && tar zxvf NoypiSSH.tgz
mv asset /home/vps/public_html
mv view /home/vps/public_html
echo "Done installing -Rodd"
