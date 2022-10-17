# Design Project 1 Testing

* For the first design project, I'm going to focus primarily on working on configuring the EDR and testing some different events in the environment. I'm not going to be performing a full blown pen-test simply because I want to research more about fully completing a pent-test and what strategies to use as I have never performed one. With that said, I'm going to be documenting some of the configurations I have made to wazuh in this document as well as some of the events I can log in Wazuh.

# Testing Wazuh's Capabilities

* First off, we have two agents added to the Wazuh Dashboard as of now, windows-1 and linux-1. Looking at the agents in the Wazuh dashboard, we see an online status, Operating system, and other simple information about the agent we added. Wazuh, by default, logs different system actions such as log ons and user creations which I detailed in my design project video. Wazuh also performs differnt CIS benchmarks against your systems to show how the current state of your systems security configurations are looking and what can be improved.

![image](https://user-images.githubusercontent.com/70913875/196075327-92fc0024-0a26-4267-8bf5-c09727875c37.png)

# Editing OSSEC.conf

* In order to make rule changes, for example if we want to enable file integrity monitoring of a certain directory, we do this in the ossec.conf file. This is located in the ossec folder and is located with the rest of the Wazuh agent files. Once we access the ossec.conf file, we are able to edit it and add different rules. I want to explore different rules that Wazuh can handle and the different things that can be monitored in ossec.conf in future design projects. 
