Vul onderstaande aan met de antwoorden op de vragen uit de readme.md file. Wil je de oplossingen file van opmaak voorzien? Gebruik dan [deze link](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) om informatie te krijgen over
opmaak met Markdown.


a) java 8 werkte niet maar met 11 wel (zie console output onderaan).
   Jenkins neemt de taal van de browser over. Dus: Instellingen --> Taal --> Alternatieven instellen... --> Selecteer een taal om toe te voegen --> Meer talen zoeken... --> English (US) --> Toevoegen --> OK


b) Er zijn 88 pluins geïnstalleerd.


c) Users zijn hier te vinden: var/lib/jenkins/users
   Naam: Jarne_9427057575369852846




sudo apt-get install jenkins
Hit:1 http://be.archive.ubuntu.com/ubuntu jammy InRelease
Get:2 http://be.archive.ubuntu.com/ubuntu jammy-updates InRelease [114 kB]                                           
Ign:3 https://pkg.jenkins.io/debian-stable binary/ InRelease                                                         
Get:4 http://be.archive.ubuntu.com/ubuntu jammy-backports InRelease [99,8 kB]                                        
Hit:5 https://pkg.jenkins.io/debian-stable binary/ Release                                           
Hit:6 https://deb.nodesource.com/node_14.x jammy InRelease                                           
Get:7 http://be.archive.ubuntu.com/ubuntu jammy-updates/main amd64 Packages [695 kB]
Hit:9 http://security.ubuntu.com/ubuntu jammy-security InRelease
Get:10 http://be.archive.ubuntu.com/ubuntu jammy-updates/main i386 Packages [371 kB]
Get:11 http://be.archive.ubuntu.com/ubuntu jammy-updates/main amd64 DEP-11 Metadata [95,1 kB]
Get:12 http://be.archive.ubuntu.com/ubuntu jammy-updates/universe amd64 DEP-11 Metadata [255 kB]
Get:13 http://be.archive.ubuntu.com/ubuntu jammy-updates/multiverse amd64 DEP-11 Metadata [940 B]
Get:14 http://be.archive.ubuntu.com/ubuntu jammy-backports/universe amd64 DEP-11 Metadata [12,6 kB]
Fetched 1.643 kB in 1s (2.541 kB/s)                               
Reading package lists... Done
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
fontconfig is already the newest version (2.13.1-4.2ubuntu5).
fontconfig set to manually installed.
openjdk-11-jre is already the newest version (11.0.16+8-0ubuntu1~22.04).
0 upgraded, 0 newly installed, 0 to remove and 28 not upgraded.
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  net-tools
The following NEW packages will be installed:
  jenkins net-tools
0 upgraded, 2 newly installed, 0 to remove and 28 not upgraded.
Need to get 0 B/93,0 MB of archives.
After this operation, 94,4 MB of additional disk space will be used.
Do you want to continue? [Y/n] y
Selecting previously unselected package net-tools.
(Reading database ... 211438 files and directories currently installed.)
Preparing to unpack .../net-tools_1.60+git20181103.0eebece-1ubuntu5_amd64.deb ...
Unpacking net-tools (1.60+git20181103.0eebece-1ubuntu5) ...
Selecting previously unselected package jenkins.
Preparing to unpack .../jenkins_2.361.3_all.deb ...
Unpacking jenkins (2.361.3) ...
Setting up net-tools (1.60+git20181103.0eebece-1ubuntu5) ...
Setting up jenkins (2.361.3) ...
Job for jenkins.service failed because the control process exited with error code.
See "systemctl status jenkins.service" and "journalctl -xeu jenkins.service" for details.
invoke-rc.d: initscript jenkins, action "start" failed.
● jenkins.service - Jenkins Continuous Integration Server
     Loaded: loaded (/lib/systemd/system/jenkins.service; enabled; vendor preset: enabled)
     Active: activating (auto-restart) (Result: exit-code) since Fri 2022-11-04 15:48:05 CET; 3ms ago
    Process: 7734 ExecStart=/usr/bin/jenkins (code=exited, status=1/FAILURE)
   Main PID: 7734 (code=exited, status=1/FAILURE)
        CPU: 67ms

nov 04 15:48:05 jarne-virtual-machine systemd[1]: Failed to start Jenkins Continuous Integration Server.
dpkg: error processing package jenkins (--configure):
 installed jenkins package post-installation script subprocess returned error exit status 1
Processing triggers for man-db (2.10.2-1) ...
Errors were encountered while processing:
 jenkins
E: Sub-process /usr/bin/dpkg returned an error code (1)

jarne@jarne-virtual-machine:~$ sudo update-alternatives --config java
There are 2 choices for the alternative java (providing /usr/bin/java).

  Selection    Path                                            Priority   Status
------------------------------------------------------------
  0            /usr/lib/jvm/java-11-openjdk-amd64/bin/java      1111      auto mode
  1            /usr/lib/jvm/java-11-openjdk-amd64/bin/java      1111      manual mode
* 2            /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java   1081      manual mode

Press <enter> to keep the current choice[*], or type selection number: 0
update-alternatives: using /usr/lib/jvm/java-11-openjdk-amd64/bin/java to provide /usr/bin/java (java) in auto mode
  
  
jarne@jarne-virtual-machine:~$ sudo apt-get install jenkins
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
jenkins is already the newest version (2.361.3).
0 upgraded, 0 newly installed, 0 to remove and 28 not upgraded.
1 not fully installed or removed.
After this operation, 0 B of additional disk space will be used.
Do you want to continue? [Y/n] y
Setting up jenkins (2.361.3) ...
