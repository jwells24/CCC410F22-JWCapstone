# Configuring Wazuh

* For this objective, I wanted to configure Wazuh a little more and make it more than the base version of Wazuh. Below, I'll document some of the configuration changes I made to Wazuh.

## Configurations

### File Integrity Monitoring

* The first thing that I attempted to configure in Wazuh is to add file integrity monitoring to a specific directory and file. I was able to do this by adding the line below to the config file of the wazuh agent. This line creates real time, filel integrity monitoring for the directory of choice. I created a directory called test and edited some files to get the following messages in Wazuh. 

* ![image](https://user-images.githubusercontent.com/70913875/206068228-d92578b8-1010-4c13-84ab-5b1d004b823e.png)

* This line was applicable for Windows 10, and worked for my windows 10 machine and I did not enable any specfic file integrity monitoring for my linux box. This configuration will be useful for monitoring specific directories that are integral to the system and being alerted when they are altered or modified. 

### Policy Monitoring

* Another facet of configuration that I looked at was policy monitoring and scanning the system for possible malware. In the rootcheck configuration portion of ossec.conf, I added the lines pictured below in order to add more substance to the policy monitoring aspect of Wazuh. I added lines that: check for windows malware, check for trojans, check all ports, and scan the entire system. I also added a frequency line to perform these operations every 24 hours on an automated basis. There is also an option in Wazuh to perform the rootcheck operations whenever necessary.

* ![image](https://user-images.githubusercontent.com/70913875/206069555-dcb6abb6-3e77-4a28-a196-340b076c4e8c.png)

* These additions will help to secure Wazuh even more, and will be applicable on both the Windows and linux ossec.conf minus the operating system specific operations. 

### New Files Monitoring

* Another facet of ossec.conf that I wanted to look into was syscheck. Besides for file integrity monitoring, there are other important settings that you can add in order to alert other things to the dashboard. One thing that I chose to add to ossec.conf, in the syscheck section, was a setting to alert the agent of any new files created in the system. This was done by inserting the line below into the syscheck portion of ossec.conf.

* ![image](https://user-images.githubusercontent.com/70913875/206071331-6b2d93a6-7d25-468e-886d-3ff665b33df6.png)

* This addition will give me even more insight into the windows and linux boxes I have configured in my environment. Any activity involving the creation of files will be logged and cause an alert to show up in the dashboard, better helping out my observations into the boxes.

