# Firefox-GNS3
This is a fork of the original "GNS3 webterm" docker
This version is completely outdated with Debian 8 and Firefox 68.9

So I decidate to create another repository, maintained by me,
with the latest package and the latest version of Debian


## HOW TO BUILD
```sh
sudo docker build -t firefox-deb10:78.4 .
```

## HOW TO USE IN GNS3
download the `webterm-updated.gns3a` and import that into your GNS3

don't forgot to configure static/dhcp into the menu
