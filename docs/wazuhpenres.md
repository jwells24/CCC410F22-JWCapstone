# Wazuh Pen Test Research & Brainstorming

* In this objective, I'm focusing on researching pen testing in general and pen testing against EDR's. I also want to start to brainstorm some tools and other vectors of attack I can use against Wazuh for my testing.

### Pen Test Research

* While conducting my research, I have added to new sources to my reference page to cover some other aspects of my introduction to creating a pen test against Wazuh. The first source I found was an interesting github blog post about some methods someone has used to attack EDR's and bypass some of their monitoring and response systems. I can use this source to add some tools and techniques to my pen testing package in order to create some methods of attack. 

* As for my second source, I am looking at a source of different pen test methods and step-by-step planning on each layer of the test. I'm going to use this source to give me more insight into actually planning the pent test and picking out a method to go for. This source will also give me some real world knowledge about actually conducting a penetration test, which will be helpful for me.

* Note: An updated reference page can be found on the Design Project 2 homepage. 

### Pen Test Brainstorming

* As for the actual penetration test, I have decided to go for a targeted testing method. This means that I will have intimate knowledge of the environment that I will be attacking, and will have a specific focus on what I am specifically going to be targeting. Using my sixth source, from Imperva, I'm going to need to follow the five steps to a penetration test. These steps are as follows

1. Planning & Reconaissance
2. Scanning
3. Gaining Access
4. Maintaining Access
5. Analysis

* Below is a very crude diagram of my environment, as I have set it up. My plan is to design methods of attack for each step of the penetration test and make sure to full document everything I do in the actual test. My main goal is to attempt to exploit all three boxes while documenting what alerts and mitigations Wazuh uses while I perform attacks on different stages of the attack. Another objective I have is to gain administrative access to one of the boxes without Wazuh being alerted, which would be interesting to document and understand for my analysis of Wazuh. Once I have completed the penetration test, as I have stated in my future plans for next semester, I am going to do a deep analysis and review for Wazuh which will be the final step in my project. 

* ![image](https://user-images.githubusercontent.com/70913875/206075958-8a1cd9a2-cae7-4a7d-9167-c38631ea9e8d.png)
