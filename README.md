# Performing-Activities-on-the-Network
I used a program named WireShark to filter and observe specific Activities going on in the background of a network using two virtual machines in the Canada Region using Azure and Remote Desktop

![Screenshot (118)](https://github.com/user-attachments/assets/52b2815b-23b0-4e8e-8da4-bc501e271e12)
These are the two Virtual Machines I set up Using the Cloud computing names Azure
# Instillation
![Screenshot (119)](https://github.com/user-attachments/assets/40486c58-5852-4934-aa27-899bfd977ef6)
This is me Downloading Wireshark


![Screenshot (120)](https://github.com/user-attachments/assets/0ef82916-2387-4517-84e7-ecc137fb86f4)
This is the Wireshark environment


![Screenshot (121)](https://github.com/user-attachments/assets/add39ee1-e12a-4c4f-af07-36fa1bb38907)
This is just the unflitered traffic that goes in the background of the Virtual Machine

# ICMP Traffic
![Screenshot (122)](https://github.com/user-attachments/assets/3bfbcc1e-2640-42ef-9424-abef37bd9547)
Here I filtered the program for icmp traffic but there is no current traffic to be observed


![Screenshot (123)](https://github.com/user-attachments/assets/55545590-d97b-49fd-a03c-4b374bbee805)
Here I used the ping command to create ICMP traffic


![Screenshot (125)](https://github.com/user-attachments/assets/a21dd5ec-3d7b-4bb2-9ec9-d9e377454849)
Here I'm looking at The Physical address in both powershell and wire shark.


![Screenshot (126)](https://github.com/user-attachments/assets/b53c665b-7a1c-4307-8497-f74c0fbeba10)
Here I'm looking at the source address


![Screenshot (127)](https://github.com/user-attachments/assets/804146c0-fa8f-4539-8d6a-c83f2c985d63)
Here I created a rule to block/deny ICMP traffic


![Screenshot (128)](https://github.com/user-attachments/assets/71d2f04a-8876-4884-af82-10a8825c6927)
Here it shows that the rule is set in place


![Screenshot (129)](https://github.com/user-attachments/assets/36246e60-1321-4611-85da-b1afbfad6f47)
It's showing here that the ICMP traffic is being blocked and isn't working anymore


![Screenshot (130)](https://github.com/user-attachments/assets/0946a662-ba4f-4ced-b14e-f271b10fc1f2)
Here it is showing that there is just request's with no response because the ICMP is being blocked by the setting in place


![Screenshot (131)](https://github.com/user-attachments/assets/3eecc809-f62d-425f-8bb0-9d04f38516a1)
Here I deleted the ICMP rule


![Screenshot (132)](https://github.com/user-attachments/assets/81d6f7cb-929c-4c60-b11d-28a826e8546a)
After the security rule has been deleted, the ping started to work again

# SSH Trafdic 
![Screenshot (133)](https://github.com/user-attachments/assets/d40441b7-2699-416b-b5fd-2a2dc25da369)
Here I am filtering for SSH traffic while i simultaneously logging into the Linux virtual machine that I have created


![Screenshot (134)](https://github.com/user-attachments/assets/8098b761-1089-4782-8494-2bc4eb7adfe1)
I used tcp.port == 22  to show that is it the same as ssh 


![Screenshot (135)](https://github.com/user-attachments/assets/753ebf8f-df16-4b15-8a89-964cb260f27e)
Here I logged out of the Linux Virtual Machine and It ended the SSH connection


![Screenshot (136)](https://github.com/user-attachments/assets/fb87a3cb-2f2b-489c-a60d-6ecbd7ff696a)
Here I created a file named dhcp, with two commands to run /release and /renew. I put it all in
one file because I when you use the release command, it will terminated the connection completely.


![Screenshot (137)](https://github.com/user-attachments/assets/19428c78-877c-44be-9f66-2902388f5a66)
You can see the connection being terminated, and reconnected after running the file

# DNS
![Screenshot (138)](https://github.com/user-attachments/assets/29678f98-d5bf-4087-980f-68f17009366c)
Here you  can see that when filtering DNS, you can see the two IP addresses are in constant contact with each other


![Screenshot (139)](https://github.com/user-attachments/assets/6ddc5edf-5b42-4ba9-9ca7-d7a53d66f625)
Here you see the same thing with a different website, Facebook
