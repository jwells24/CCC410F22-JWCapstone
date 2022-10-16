# Design Project 1 Environment

* For the first design project, I wanted to keep it simple and create an environment with only two endpoints to represent someones home. This environment is going to consist simply of a windows 10 machine and a CentOS machine as endpoints. Wazuh requires 3 components to be installed on a central machine for their service so I'm also going to have a windows 10 machine acting as the host for the Wazuh Server, dashboard, and indexer. 

## Network

* I am going to use VMware Workstation to host the virtual machines for this project. Below are the hostnames of the machines that I have created, a network assignment, and a brief description of their purpose. 

1. linux-1 - 185.12.13.5 - This box is a CentOS 7 box and is an going to be used as an endpoint on the network.
2. windows-1 - 185.12.13.4 - This box is a Windows 10 box and is going to be used as an endpoint on the network.
3. wazuh-1 - 185.12.13.3 - This box is a CentOS 7 box and is going to be used as a host for Wazuh Server, Wazuh Indexer, and the Wazuh Dashboard. 
