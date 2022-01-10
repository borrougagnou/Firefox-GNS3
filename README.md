# Intro
This is a fork of the original "GNS3 webterm" docker
The original version is completely outdated with Debian 8 and Firefox 68.9

So I decidate to create another repository, maintained by me,
with the latest package and the latest version of Debian

## changelog:
#### 20220110:
- create tag `firefox-gns3:buster` and `firefox-gns3:bullseye`
- [latest] update from debian buster to debian bullseye (Firefox 78 esr --> Firefox 91 esr)
- [buster] Firefox 78.4.0esr --> Firefox 78.15.0esr

__I think improve this Dockerfile, because actually it download a lot of layer...__
__For any question/suggestion/improvement, don't hesitate to create issue.__

# Installation
### Easy install :
Download the file [webterm-updated.gns3a](https://github.com/borrougagnou/Firefox-GNS3/releases/latest/download/webterm-updated.gns3a)

Open GNS3 --> New Template --> Import an appliance file (.gns3a extension) --> choose a server --> Finish

don't forgot to configure static/dhcp


### Manual install :
Import the [Dockerfile](https://github.com/borrougagnou/Firefox-GNS3/releases/latest/download/Dockerfile) into the GNS3 VM Server

and follow the GNS3 manual: https://docs.gns3.com/docs/emulators/create-a-docker-container-for-gns3/

don't forgot to configure static/dhcp into the menu


# Screenshot
Fortigate 6.x problem is now solved ! :) 
![screenshot-VNC](https://user-images.githubusercontent.com/10796546/97975437-6d0afa00-1dc9-11eb-8f5a-a17e3a315412.png)
