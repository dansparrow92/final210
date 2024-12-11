# This is a Linux/GNU installation using automated scripts

#In the VMware workstation select debian ISO image
on the preconfig window type "https://phillipsd.com/210/f24sda.cfg" to give the installation process

#we use the sda.cfg file because the VM workstation recognizes the virtual machines as hardware
on the debian gnu/linux interface without a GUI we use command 
wget phillipsd.com/210/post_run

run command "bash post_get" which will install a series of things including 

empty passphrase when prompted!

this screenshot shows a ssh connection from my host machine to my virtal machine

![image](https://github.com/user-attachments/assets/337cfc8e-17d9-4f4f-96b3-bddc45880761)

#starting the allocated spaces in KVM

added a virtual disk with 5gb of allocated memory

![image](https://github.com/user-attachments/assets/deb2a7e8-daee-4311-9a08-721968f850a0)

ran fdisk /dev/vdb
run fdisk /degv/vdc
to create two lvms

![image](https://github.com/user-attachments/assets/0bbed123-50db-4cd6-8c06-68d552667286)

sudo pvdisplay

![image](https://github.com/user-attachments/assets/772f3b0e-c396-4edf-9d09-e42fdfb6d890)

running sudo vgcreate datavg /dev/vdb1 /dev/vdc1

![image](https://github.com/user-attachments/assets/9b4b3c4d-663f-4d63-b103-c85ff541fba3)

running sudo vgscan displays

![image](https://github.com/user-attachments/assets/7dcc318d-51a5-4a2d-844b-45c8e2d1454b)

create lvcreate --name datallv --size 2G datavg

![image](https://github.com/user-attachments/assets/2c0337e0-13a5-4550-bbc7-1161d8a61c82)


sudo lvs

![image](https://github.com/user-attachments/assets/8c85c4ee-c24f-4976-b29f-83d9a0b7cf02)

sudo lvscan

![image](https://github.com/user-attachments/assets/6cd16358-d16b-4791-9a2d-7608a0ddf94b)

sudo mkdir /mnt/data1 /mnt/data2 /mnt/data3
sudo ls -l /mnt

#shows mounted
![image](https://github.com/user-attachments/assets/a0c4b8d1-59cc-4bd0-9562-8c722b9e65f2)


cat /etc/fstab to change the UUID

![image](https://github.com/user-attachments/assets/19ffc1d9-32cd-4ec7-b405-f8ccd67fbbed)


![image](https://github.com/user-attachments/assets/6c8759ac-7226-4ce3-a6fe-3cff88934e13)

#finished server gnu

![image](https://github.com/user-attachments/assets/16c834f4-af5f-4ebf-b000-903b9b70e772)

#adding a user named tux1

![image](https://github.com/user-attachments/assets/52df94cf-1b52-405c-96bc-726569bfed46)


#note most of this stuffs "whys" are somewhat of a mystery to me but going through the steps of setting up this machine to function properly was i think a eye opening experience and it does inspire me to dig into the world of Linux seeing how much i dont know and how many questions i cannot answer without guidance.







