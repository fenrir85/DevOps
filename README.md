# DevOps

This repository is Casptone Project for bootcamp ITJ Devops

Github Action use Folder Capstone Project execute tests 
if pass then build docker to my docker hub named  fenrius85 / capstone-devops

You can use the image with this commands on windows powershell
docker pull fenrius85/capstone-devops
docker run -p 3000:3000 fenrius85/capstone-devops

now you can see node app running
http://localhost:3000/
![image](https://user-images.githubusercontent.com/1261774/232397929-17e2d7ce-bf89-455f-9c5e-edb2da418382.png)


for ansible use clone repo https://github.com/fenrir85/DevOps.git
on folder Capstone-project you can find a file docker-compose
use docker-compose up

on ansible_controller terminal
cd ansible_files && ansible-playbook -i inventory.ini playbook.yml

![image](https://user-images.githubusercontent.com/1261774/232397781-5dc712e6-75e4-4456-9e53-63869d0aac68.png)
![image](https://user-images.githubusercontent.com/1261774/232398040-9e856819-ae2c-4ced-a0ce-f901a9e944f2.png)

Special Thanks to ITJuana Bootcamp Instructors
