
# PART 1: BUILD THE NETWORK

<img width="550" height="357" alt="image" src="https://github.com/user-attachments/assets/9294b8ff-6de2-4f4e-95f1-342cb3684c9b" />
Super basic


#Step 2: Connect everything

<img width="471" height="395" alt="image" src="https://github.com/user-attachments/assets/209b4054-5947-4b6e-8a47-9b5e92d052c7" />


Step 3: Configuring the router to assign some IP addresses 

<img width="746" height="619" alt="image" src="https://github.com/user-attachments/assets/0d4cf4b6-273f-4e55-b27d-4ea5745ca298" />


Commands used:



enable

configure terminal

interface g0/0

ip address 192.168.1.1 255.255.255.0

no shutdown


Router is now reachable by the network 


<img width="426" height="363" alt="image" src="https://github.com/user-attachments/assets/f4fdefc8-1632-4d90-a0cf-3860f39f5e10" />



Next, we will configure a DHCP server to hand out a few IP addresses automatically

<img width="668" height="321" alt="image" src="https://github.com/user-attachments/assets/85832311-6fee-4de9-aca8-2c38de897a0a" />

made  192.168.1.100 the static address to assign to the thing from  


Next, we will set the PC's to use DHCP as well 

<img width="160" height="238" alt="image" src="https://github.com/user-attachments/assets/e5318f16-27a4-4096-9dff-cc838130f7e4" />

Next, we'll use ping to test connectivity in the network 

ping 192.168.1.1 

This ping failed  😢

# Part 2: Identify the Issue 

Start with 


ipconfig 

<img width="364" height="262" alt="image" src="https://github.com/user-attachments/assets/cd0a7b2a-f17c-46d0-a8d5-206b9bcea872" />

Apipa Addresses on both devices 


This points to a failure with the DHCP server!





















