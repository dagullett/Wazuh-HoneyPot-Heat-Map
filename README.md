# Wazuh Honey Pot Heat Map

![Screenshot 2024-02-05 103100](https://github.com/dagullett/Wazuh-HoneyPot-Heat-Map/assets/75142644/9f2eaad4-4a8f-4a5a-a0a6-08f9d4fd1d67)


## Introduction

In this lab, I wanted to show, just how vulnerable a computer can be if it is not protected by a firewall. In this instance, I used an uBuntu server with minimum specs. The machine itself did not have a firewall. I also did not put it behind a network firewall, so that it would be completely exposed to neerdowells on the internet. This lab is showcasing the results in a graphical matter. In this lab we will:

- Create 2 virtual machines in the cloud
- Install Wazuh dashboard and install Wazuh agent
- Ingest logs of Password guessing, brute force attacks, and ssh connection attempts
- Create Heat Map of Attack Locations

## Setup

![Screenshot 2024-02-05 185248](https://github.com/dagullett/Wazuh-HoneyPot-Heat-Map/assets/75142644/fb6b83cf-fa05-410d-8276-b0833dd842b3)


![Screenshot 2024-02-05 185224](https://github.com/dagullett/Wazuh-HoneyPot-Heat-Map/assets/75142644/8e1febc2-793d-42e2-8451-8a1cdb303fcd)

The first thing I did was create two virtual machines. One machine had the minimum specs to download and operate the Wazuh dashboard while the other had the minimum specs to download the wazuh agent. I then had to create a firewall rule so that the Wazuh agent could successfully communicate with the Wazuh dashboard while also protecting the dashboard from behind a firewall. I left one machine completely exposed to the internet.

## The Attack


![Screenshot 2024-02-05 100943](https://github.com/dagullett/Wazuh-HoneyPot-Heat-Map/assets/75142644/9b33c6ea-ec52-4212-a866-9c8a2bba30bc)

The first attacks started coming from Shanghai, China. They ultimately wanted to get into the machine more than any other location. Comparatively to the other nations in the world, they tried to get in over 4,000 times while other places tried a few hundred to just a couple. The most common types of attack were password guessing, ssh connection attempts, and brute force attacks.

![Screenshot 2024-02-05 184312](https://github.com/dagullett/Wazuh-HoneyPot-Heat-Map/assets/75142644/0cdb98c8-811b-485a-8f53-97dbeaff4d7a)

They never stopped either. The attacks went on for over 24 hours. The biggest attempts were around Midnight eastern time. I assume that's when China is most awake trying to attack.

![Screenshot 2024-02-05 184244](https://github.com/dagullett/Wazuh-HoneyPot-Heat-Map/assets/75142644/68ab6bc4-a701-4409-bbb5-12ecdd011c80)

![Screenshot 2024-02-05 184340](https://github.com/dagullett/Wazuh-HoneyPot-Heat-Map/assets/75142644/d1bc6b6d-b74d-4fab-8002-7d969b0c029e)

The attacks weren't just foreign either. My machine was also attacked several hundred times from my own backyard of the United States. States such as New York, Kansas, and Florida were some of the bigger contributors of the attack.

## Heat Map

![Screenshot 2024-02-05 184457](https://github.com/dagullett/Wazuh-HoneyPot-Heat-Map/assets/75142644/c0848d96-ec86-4a96-9f20-b2e126689986)

Everyone all over the world tried to get into my machine. The only places I didn't see activity was from Africa and Antartica. The most attacks came from China, Unite States, and Japan. China won overall. They are the only area to have over 2,000 attacks. 

![Screenshot 2024-02-05 184755](https://github.com/dagullett/Wazuh-HoneyPot-Heat-Map/assets/75142644/cf743efa-1674-480f-a68b-dd54268158b8)

## Conclusion

This lab was very eye opening. It really shows the importance of protecting your systems from the internet. You don't realize how many people are lurking and trying to get into your machines. Be safe and protect yourself with a firewall.
