# This is a Linux/GNY installation using automated scripts

#In the VMware workstation select debian ISO image
on the preconfig window type "https://phillipsd.com/210/f24sda.cfg" to give the installation process

#we use the sda.cfg file because the VM workstation recognizes the virtual machines as hardware
on the debian gnu/linux interface without a GUI we use command 
wget phillipsd.com/210/post_run

run command "bash post_get" which will install a series of things including 

empty passphrase when prompted
this screenshot shows a ssh connection from my host machine to my virtal machine
![image](https://github.com/user-attachments/assets/337cfc8e-17d9-4f4f-96b3-bddc45880761)

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

sudo lvs
![image](https://github.com/user-attachments/assets/8c85c4ee-c24f-4976-b29f-83d9a0b7cf02)

sudo lvscan
![image](https://github.com/user-attachments/assets/6cd16358-d16b-4791-9a2d-7608a0ddf94b)




![image](https://github.com/user-attachments/assets/c20cc552-555b-412d-8a92-659d084f502b)



