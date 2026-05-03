# Active-Directory

## Objective

Active Directory’s objective is to centrally manage and secure users, computers, and resources in a Windows domain by providing authentication, authorization, and policy enforcement.

### Skills Learned

- Strong understanding of structures of the domain and centralized identity management
- Proficiency in configuring and managing users, groups and access permissions
- Skilled in analyzing authentication logs to detect suspicious or unauthorized activity
- Knowledge of common Active Directory attack paths and priviledges escalating techniques
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- 
- 
- 

## Steps
1.I built a diagram using draw.io to help me understand how data might flow and how pieces are strung together
<img width="300" height="400" alt="Screenshot_3-5-2026_185318_app diagrams net" src="https://github.com/user-attachments/assets/96f24f9e-a886-44d9-a4f7-80d765830178" />

2.I created three virtual machines in the vultr cloud to help me carry out this project
  The first machine is the test machine and I used the windows 10 server
  The second machine is the active directory machine and I used the windows 10 server again
  The third machine is the Splunk machine and i used Ubuntu server
<img width="300" height="400" alt="creating 3 virtual machines" src="https://github.com/user-attachments/assets/1d541e76-cc01-45f7-b432-080e0fe24580" />

3.I created a firewall group and added my three machines to the firewall group so that thry will be protected from invaders.
<img width="400" height="450" alt="creating firewall group" src="https://github.com/user-attachments/assets/03185317-67b6-408a-95a6-c68cea0dc4b0" /><img width="200" height="300" alt="adding firewalls to my vms" src="https://github.com/user-attachments/assets/bb49456a-e42f-4ffe-bca4-ba9906445190" /><img width="200" height="300" alt="Screenshot_3-5-2026_19418_console vultr com" src="https://github.com/user-attachments/assets/3899232a-9405-4512-ba60-9a4236dfce59" /><img width="200" height="300" alt="Screenshot_3-5-2026_194142_console vultr com" src="https://github.com/user-attachments/assets/644c2097-8bff-4534-854f-3d65e9cba459" />

4.I also did an extra configuration by creating and adding my virtual machines to the VPC Network
<img width="300" height="400" alt="vpc" src="https://github.com/user-attachments/assets/d3e4a061-3982-46d8-a2e5-66511f9a2b25" />

5.I checked my connectivity because all my virtual machines should be able to communicate with one another. Thre was no connectivity and in my case that is a huge problem.
 <img width="300" height="400" alt="something wrong" src="https://github.com/user-attachments/assets/f0ed88aa-aa23-4218-b8e6-80b408011183" />

 6.I found my problem in the second ethernet the ip address there is 169 address not 10.x.x address and i fixed that by going to the network settings and changing the adapter options of ethernet 0.2's ipv4 properties by adding my ip and subnet address
<img width="1280" height="960" alt="foundissue" src="https://github.com/user-attachments/assets/8b6e77c1-4ae0-4fe0-bab3-02cc27546aa9" /><img width="200" height="300" alt="troubleshoot" src="https://github.com/user-attachments/assets/22763caf-2c4c-4f8a-9dfd-80758f53bce3" />


7.My problem was therefore fixed because there was connectivity between my virtual machines
<img width="200" height="300" alt="problemfixed" src="https://github.com/user-attachments/assets/1fe7142d-3b87-477f-b076-420590c22b4c" />






