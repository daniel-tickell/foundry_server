Files used in creating a Foundry instance.


To create a new instance we will call this one test

1. Create a new directory 'mkdir ~/foundry_test'
2. make the foundryvtt directory 'mkdir ~/foundry_test/foundryvtt'
3. download and install the foundry ZIP file, then copy it to the foundryvtt dir
4. unzip the Foundry*.zip file
5. make a copy of start.sh in ~/foundry_test
6. Edit the start.sh file to point to the new directory name
7. chmod +x start.sh
8. run start.sh and configure foundry (this will create the foundrydata directory
9. run ~/copy_certs.sh
10. run 'ln -s ~/tokens_shared ~/foundry_test/foundrydata/Data/tokens_shared'
11. Create a new file with contents of foundry.service 'sudo touch /etc/systemd/system/foundry_test.service'
12. Edit that file and update the dir name
13. run 'Sudo systemctl enable foundry_test.service'
14. run 'Sudo systemctl start foundry_test.service'

