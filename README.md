# Intro
This is a fork of the original "GNS3 webterm" docker
The original version is completely outdated with Debian 8 and Firefox 68.9

So I choose to do another repository, maintained by me,
with the latest package and the latest version of Debian

|      Tag       |  Debian Version  |    Firefox  Version    |
| :---           | :---             | :---                   |
| `latest`       | 12.9  (Bookworm) | Firefox  128.7.0esr    |
| `bookworm`     | 12.9  (Bookworm) | Firefox  128.7.0esr    |
| `bullseye`     | 11.11 (Bullseye) | Firefox  128.7.0esr    |
| `buster`       | 10.13 (Buster)   | Firefox  115.12.0esr   |
| `stretch`      | 9.13  (Stretch)  | Firefox  91.11.0esr    |
| `experimental` | 12.9  (Bookworm) | Firefox  Nightly 137.0 |

## changelog:
#### 20250214
- Update image and Firefox version
- [bookworm/latest] Debian 12.2 to 12.9 | Firefox 128.7.0esr
- [bullseye] Debian 11.8 to 11.11 | Firefox 115.5.0esr to 128.7.0esr
- [buster] Firefox 115.5.0esr to 115.12.0esr
- [experimental] Debian 12.2 to 12.9 | Firefox Nightly 122.0a0 to 137.0a1

#### 20231129
- create tag `experimental`
- [experimental] Implement Firefox Nightly 122.0a0 from Mozilla[ ¹](https://blog.nightly.mozilla.org/2023/10/30/introducing-mozillas-firefox-nightly-deb-packages-for-debian-based-linux-distributions/) repository

#### 20231128
- create tag `firefox-gns3:bookworm`
- added iputils-ping package in all image.
- bump dumb-init v1.2.2 --> v1.2.5
- created multiple "gns3a" (one for each debian version)
- [latest] update from debian bullseye to debian bookworm
- [bookworm/latest] Debian 12.2 | Firefox 115.5.0esr
- [bullseye] Debian 11.6 to 11.8 | Firefox 102.8.0esr to 115.5.0esr
- [buster] Firefox 102.8.0esr to 115.5.0esr
- [stretch] I use now archive.debian.org[ ¹](https://lists.debian.org/debian-devel-announce/2023/03/msg00006.html)
- Docker `MAINTAINER`[ ³](https://docs.docker.com/engine/reference/builder/#maintainer-deprecated) is deprecated, `LABEL` is used instead.

#### 20230218
- [bullseye/latest] update to debian 11.6 with Firefox 102.8.0esr
- [buster] update to debian 10.13 with Firefox 102.8.0esr
- [stretch] added support for debian stretch 9.13 with Firefox 91.11.0

#### 20220110
- create tag `firefox-gns3:buster` and `firefox-gns3:bullseye`
- [latest] update from debian buster to debian bullseye (Firefox 78 esr --> Firefox 91 esr)
- [buster] Firefox 78.4.0esr --> Firefox 78.15.0esr

#### future changelog not yet implemented
- [buster] I use now archive.debian.org[ ¹](https://lists.debian.org/debian-devel-announce/2024/03/msg00003.html)


__I think improve this Dockerfile, because actually it download a lot of layer...__
__For any question/suggestion/improvement, don't hesitate to create issue.__

# Installation
### Easy install :
Download the file [webterm-latest.gns3a](https://github.com/borrougagnou/Firefox-GNS3/releases/latest/download/webterm-latest.gns3a)

Open GNS3 --> New Template --> Import an appliance file (.gns3a extension) --> choose a server --> Finish

don't forgot to configure static/dhcp


### Manual install :
Import the [Dockerfile](https://github.com/borrougagnou/Firefox-GNS3/releases/latest/download/Dockerfile) into the GNS3 VM Server

and follow the GNS3 manual: https://docs.gns3.com/docs/emulators/create-a-docker-container-for-gns3/

don't forgot to configure static/dhcp into the menu


# Screenshot
Fortigate 6.x problem is now solved ! :) 
![screenshot-VNC](https://user-images.githubusercontent.com/10796546/97975437-6d0afa00-1dc9-11eb-8f5a-a17e3a315412.png)
