*********** MINGW64 ~
$ pwd
/c/Users/CLS-PC
## Connect to your instance with your key pair and username here
*********** MINGW64 ~$ `ssh -i pbl2.pem ubuntu@ec2-34-211-170-9.us-west-2.compute.amazonaws.com`
The authenticity of host 'ec2-34-211-170-9.us-west-2.compute.amazonaws.com (34.211.170.9)' can't be established.
ED25519 key fingerprint is SHA256:rtdheIojQkAzd+9ShGPvHhKQGHuRXSxwUqtN20TjHfQ.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added 'ec2-34-211-170-9.us-west-2.compute.amazonaws.com' (ED25519) to the list of known hosts.
Welcome to Ubuntu 22.04.3 LTS (GNU/Linux 6.2.0-1017-aws x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

  System information as of Mon Jan 29 10:17:10 UTC 2024

  System load:  0.0               Processes:             96
  Usage of /:   20.5% of 7.57GB   Users logged in:       0
  Memory usage: 21%               IPv4 address for eth0: 172.31.23.206
  Swap usage:   0%

Expanded Security Maintenance for Applications is not enabled.

0 updates can be applied immediately.

Enable ESM Apps to receive additional future security updates.
See https://ubuntu.com/esm or run: sudo pro status


The list of available updates is more than a week old.
To check for new updates run: sudo apt update


The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

To run a command as administrator (user "root"), use "sudo <command>".
See "man sudo_root" for details.
## Update Running tools once you connect to your Ubuntu instance
ubuntu@ip-172-31-23-206:~$ sudo apt update
Hit:1 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy InRelease
Get:2 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates InRelease [119 kB]
Get:3 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-backports InRelease [109 kB]
Get:4 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/universe amd64 Packages [14.1 MB]
Get:5 http://security.ubuntu.com/ubuntu jammy-security InRelease [110 kB]
Get:6 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/universe Translation-en [5652 kB]
Get:7 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/universe amd64 c-n-f Metadata [286 kB]
Get:8 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/multiverse amd64 Packages [217 kB]
Get:9 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/multiverse Translation-en [112 kB]
Get:10 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/multiverse amd64 c-n-f Metadata [8372 B]
Get:11 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 Packages [1320 kB]
Get:12 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main Translation-en [267 kB]
Get:13 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/restricted amd64 Packages [1334 kB]
Get:14 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/restricted Translation-en [218 kB]
Get:15 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/universe amd64 Packages [1036 kB]
Get:16 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/universe Translation-en [232 kB]
Get:17 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/universe amd64 c-n-f Metadata [22.1 kB]
Get:18 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/multiverse amd64 Packages [42.1 kB]
Get:19 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/multiverse Translation-en [10.1 kB]
Get:20 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/multiverse amd64 c-n-f Metadata [472 B]
Get:21 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-backports/main amd64 Packages [41.7 kB]
Get:22 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-backports/main Translation-en [10.5 kB]
Get:23 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-backports/main amd64 c-n-f Metadata [388 B]
Get:24 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-backports/restricted amd64 c-n-f Metadata [116 B]
Get:25 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-backports/universe amd64 Packages [24.2 kB]
Get:26 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-backports/universe Translation-en [16.5 kB]
Get:27 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-backports/universe amd64 c-n-f Metadata [644 B]
Get:28 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-backports/multiverse amd64 c-n-f Metadata [116 B]
Get:29 http://security.ubuntu.com/ubuntu jammy-security/main amd64 Packages [1103 kB]
Get:30 http://security.ubuntu.com/ubuntu jammy-security/main Translation-en [207 kB]
Get:31 http://security.ubuntu.com/ubuntu jammy-security/restricted amd64 Packages [1306 kB]
Get:32 http://security.ubuntu.com/ubuntu jammy-security/restricted Translation-en [213 kB]
Get:33 http://security.ubuntu.com/ubuntu jammy-security/universe amd64 Packages [835 kB]
Get:34 http://security.ubuntu.com/ubuntu jammy-security/universe Translation-en [159 kB]
Get:35 http://security.ubuntu.com/ubuntu jammy-security/universe amd64 c-n-f Metadata [16.8 kB]
Get:36 http://security.ubuntu.com/ubuntu jammy-security/multiverse amd64 Packages [37.1 kB]
Get:37 http://security.ubuntu.com/ubuntu jammy-security/multiverse Translation-en [7476 B]
Get:38 http://security.ubuntu.com/ubuntu jammy-security/multiverse amd64 c-n-f Metadata [260 B]
Fetched 29.2 MB in 5s (5319 kB/s)
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
57 packages can be upgraded. Run 'apt list --upgradable' to see them.
### First step once we are connected to our instance ,We install a webserver called `nginx`.
ubuntu@ip-172-31-23-206:~$ `sudo apt install nginx`
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  fontconfig-config fonts-dejavu-core libdeflate0 libfontconfig1 libgd3 libjbig0
  libjpeg-turbo8 libjpeg8 libnginx-mod-http-geoip2 libnginx-mod-http-image-filter
  libnginx-mod-http-xslt-filter libnginx-mod-mail libnginx-mod-stream
  libnginx-mod-stream-geoip2 libtiff5 libwebp7 libxpm4 nginx-common nginx-core
Suggested packages:
  libgd-tools fcgiwrap nginx-doc ssl-cert
The following NEW packages will be installed:
  fontconfig-config fonts-dejavu-core libdeflate0 libfontconfig1 libgd3 libjbig0
  libjpeg-turbo8 libjpeg8 libnginx-mod-http-geoip2 libnginx-mod-http-image-filter
  libnginx-mod-http-xslt-filter libnginx-mod-mail libnginx-mod-stream
  libnginx-mod-stream-geoip2 libtiff5 libwebp7 libxpm4 nginx nginx-common nginx-core
0 upgraded, 20 newly installed, 0 to remove and 57 not upgraded.
Need to get 2692 kB of archives.
After this operation, 8345 kB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 fonts-dejavu-core all 2.37-2build1 [1041 kB]
Get:2 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 fontconfig-config all 2.13.1-4.2ubuntu5 [29.1 kB]
Get:3 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libdeflate0 amd64 1.10-2 [70.9 kB]
Get:4 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libfontconfig1 amd64 2.13.1-4.2ubuntu5 [131 kB]
Get:5 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libjpeg-turbo8 amd64 2.1.2-0ubuntu1 [134 kB]
Get:6 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libjpeg8 amd64 8c-2ubuntu10 [2264 B]
Get:7 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 libjbig0 amd64 2.1-3.1ubuntu0.22.04.1 [29.2 kB]
Get:8 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 libwebp7 amd64 1.2.2-2ubuntu0.22.04.2 [206 kB]
Get:9 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 libtiff5 amd64 4.3.0-6ubuntu0.7 [185 kB]
Get:10 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 libxpm4 amd64 1:3.5.12-1ubuntu0.22.04.2 [36.7 kB]
Get:11 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libgd3 amd64 2.3.0-2ubuntu2 [129 kB]
Get:12 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 nginx-common all 1.18.0-6ubuntu14.4 [40.0 kB]
Get:13 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 libnginx-mod-http-geoip2 amd64 1.18.0-6ubuntu14.4 [11.9 kB]
Get:14 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 libnginx-mod-http-image-filter amd64 1.18.0-6ubuntu14.4 [15.4 kB]
Get:15 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 libnginx-mod-http-xslt-filter amd64 1.18.0-6ubuntu14.4 [13.7 kB]
Get:16 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 libnginx-mod-mail amd64 1.18.0-6ubuntu14.4 [45.7 kB]
Get:17 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 libnginx-mod-stream amd64 1.18.0-6ubuntu14.4 [72.9 kB]
Get:18 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 libnginx-mod-stream-geoip2 amd64 1.18.0-6ubuntu14.4 [10.1 kB]
Get:19 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 nginx-core amd64 1.18.0-6ubuntu14.4 [484 kB]
Get:20 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 nginx amd64 1.18.0-6ubuntu14.4 [3872 B]
Fetched 2692 kB in 0s (38.2 MB/s)
Preconfiguring packages ...
Selecting previously unselected package fonts-dejavu-core.
(Reading database ... 64799 files and directories currently installed.)
Preparing to unpack .../00-fonts-dejavu-core_2.37-2build1_all.deb ...
Unpacking fonts-dejavu-core (2.37-2build1) ...
Selecting previously unselected package fontconfig-config.
Preparing to unpack .../01-fontconfig-config_2.13.1-4.2ubuntu5_all.deb ...
Unpacking fontconfig-config (2.13.1-4.2ubuntu5) ...
Selecting previously unselected package libdeflate0:amd64.
Preparing to unpack .../02-libdeflate0_1.10-2_amd64.deb ...
Unpacking libdeflate0:amd64 (1.10-2) ...
Selecting previously unselected package libfontconfig1:amd64.
Preparing to unpack .../03-libfontconfig1_2.13.1-4.2ubuntu5_amd64.deb ...
Unpacking libfontconfig1:amd64 (2.13.1-4.2ubuntu5) ...
Selecting previously unselected package libjpeg-turbo8:amd64.
Preparing to unpack .../04-libjpeg-turbo8_2.1.2-0ubuntu1_amd64.deb ...
Unpacking libjpeg-turbo8:amd64 (2.1.2-0ubuntu1) ...
Selecting previously unselected package libjpeg8:amd64.
Preparing to unpack .../05-libjpeg8_8c-2ubuntu10_amd64.deb ...
Unpacking libjpeg8:amd64 (8c-2ubuntu10) ...
Selecting previously unselected package libjbig0:amd64.
Preparing to unpack .../06-libjbig0_2.1-3.1ubuntu0.22.04.1_amd64.deb ...
Unpacking libjbig0:amd64 (2.1-3.1ubuntu0.22.04.1) ...
Selecting previously unselected package libwebp7:amd64.
Preparing to unpack .../07-libwebp7_1.2.2-2ubuntu0.22.04.2_amd64.deb ...
Unpacking libwebp7:amd64 (1.2.2-2ubuntu0.22.04.2) ...
Selecting previously unselected package libtiff5:amd64.
Preparing to unpack .../08-libtiff5_4.3.0-6ubuntu0.7_amd64.deb ...
Unpacking libtiff5:amd64 (4.3.0-6ubuntu0.7) ...
Selecting previously unselected package libxpm4:amd64.
Preparing to unpack .../09-libxpm4_1%3a3.5.12-1ubuntu0.22.04.2_amd64.deb ...
Unpacking libxpm4:amd64 (1:3.5.12-1ubuntu0.22.04.2) ...
Selecting previously unselected package libgd3:amd64.
Preparing to unpack .../10-libgd3_2.3.0-2ubuntu2_amd64.deb ...
Unpacking libgd3:amd64 (2.3.0-2ubuntu2) ...
Selecting previously unselected package nginx-common.
Preparing to unpack .../11-nginx-common_1.18.0-6ubuntu14.4_all.deb ...
Unpacking nginx-common (1.18.0-6ubuntu14.4) ...
Selecting previously unselected package libnginx-mod-http-geoip2.
Preparing to unpack .../12-libnginx-mod-http-geoip2_1.18.0-6ubuntu14.4_amd64.deb ...
Unpacking libnginx-mod-http-geoip2 (1.18.0-6ubuntu14.4) ...
Selecting previously unselected package libnginx-mod-http-image-filter.
Preparing to unpack .../13-libnginx-mod-http-image-filter_1.18.0-6ubuntu14.4_amd64.deb ...
Unpacking libnginx-mod-http-image-filter (1.18.0-6ubuntu14.4) ...
Selecting previously unselected package libnginx-mod-http-xslt-filter.
Preparing to unpack .../14-libnginx-mod-http-xslt-filter_1.18.0-6ubuntu14.4_amd64.deb ...
Unpacking libnginx-mod-http-xslt-filter (1.18.0-6ubuntu14.4) ...
Selecting previously unselected package libnginx-mod-mail.
Preparing to unpack .../15-libnginx-mod-mail_1.18.0-6ubuntu14.4_amd64.deb ...
Unpacking libnginx-mod-mail (1.18.0-6ubuntu14.4) ...
Selecting previously unselected package libnginx-mod-stream.
Preparing to unpack .../16-libnginx-mod-stream_1.18.0-6ubuntu14.4_amd64.deb ...
Unpacking libnginx-mod-stream (1.18.0-6ubuntu14.4) ...
Selecting previously unselected package libnginx-mod-stream-geoip2.
Preparing to unpack .../17-libnginx-mod-stream-geoip2_1.18.0-6ubuntu14.4_amd64.deb ...
Unpacking libnginx-mod-stream-geoip2 (1.18.0-6ubuntu14.4) ...
Selecting previously unselected package nginx-core.
Preparing to unpack .../18-nginx-core_1.18.0-6ubuntu14.4_amd64.deb ...
Unpacking nginx-core (1.18.0-6ubuntu14.4) ...
Selecting previously unselected package nginx.
Preparing to unpack .../19-nginx_1.18.0-6ubuntu14.4_amd64.deb ...
Unpacking nginx (1.18.0-6ubuntu14.4) ...
Setting up libxpm4:amd64 (1:3.5.12-1ubuntu0.22.04.2) ...
Setting up libdeflate0:amd64 (1.10-2) ...
Setting up nginx-common (1.18.0-6ubuntu14.4) ...
Created symlink /etc/systemd/system/multi-user.target.wants/nginx.service → /lib/systemd/system/nginx.service.
Setting up libjbig0:amd64 (2.1-3.1ubuntu0.22.04.1) ...
Setting up libnginx-mod-http-xslt-filter (1.18.0-6ubuntu14.4) ...
Setting up fonts-dejavu-core (2.37-2build1) ...
Setting up libjpeg-turbo8:amd64 (2.1.2-0ubuntu1) ...
Setting up libwebp7:amd64 (1.2.2-2ubuntu0.22.04.2) ...
Setting up libnginx-mod-http-geoip2 (1.18.0-6ubuntu14.4) ...
Setting up libjpeg8:amd64 (8c-2ubuntu10) ...
Setting up libnginx-mod-mail (1.18.0-6ubuntu14.4) ...
Setting up fontconfig-config (2.13.1-4.2ubuntu5) ...
Setting up libnginx-mod-stream (1.18.0-6ubuntu14.4) ...
Setting up libtiff5:amd64 (4.3.0-6ubuntu0.7) ...
Setting up libfontconfig1:amd64 (2.13.1-4.2ubuntu5) ...
Setting up libnginx-mod-stream-geoip2 (1.18.0-6ubuntu14.4) ...
Setting up libgd3:amd64 (2.3.0-2ubuntu2) ...
Setting up libnginx-mod-http-image-filter (1.18.0-6ubuntu14.4) ...
Setting up nginx-core (1.18.0-6ubuntu14.4) ...
 * Upgrading binary nginx                                                               [ OK ]
Setting up nginx (1.18.0-6ubuntu14.4) ...
Processing triggers for ufw (0.36.1-4ubuntu0.1) ...
Processing triggers for man-db (2.10.2-1) ...
Processing triggers for libc-bin (2.35-0ubuntu3.4) ...
Scanning processes...
Scanning linux images...

Running kernel seems to be up-to-date.

No services need to be restarted.

No containers need to be restarted.

No user sessions are running outdated binaries.

No VM guests are running outdated hypervisor (qemu) binaries on this host.

## Check Status to see if it is running bellow , running is usually in green
ubuntu@ip-172-31-23-206:~$ `sudo systemctl status nginx`
● nginx.service - A high performance web server and a reverse proxy server
     Loaded: loaded (/lib/systemd/system/nginx.service; enabled; vendor preset: enabled)
     Active: active `(running)` since Mon 2024-01-29 10:20:11 UTC; 2min 57s ago
       Docs: man:nginx(8)
    Process: 2090 ExecStartPre=/usr/sbin/nginx -t -q -g daemon on; master_process on; (code=ex>
    Process: 2097 ExecStart=/usr/sbin/nginx -g daemon on; master_process on; (code=exited, sta>
   Main PID: 2205 (nginx)
      Tasks: 2 (limit: 1121)
     Memory: 4.3M
        CPU: 25ms
     CGroup: /system.slice/nginx.service
             ├─2205 "nginx: master process /usr/sbin/nginx -g daemon on; master_process on;"
             └─2208 "nginx: worker process" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "">

Jan 29 10:20:11 ip-172-31-23-206 systemd[1]: Starting A high performance web server and a reve>
Jan 29 10:20:11 ip-172-31-23-206 systemd[1]: Started A high performance web server and a rever>
lines 1-16/16 (END)...skipping...
● nginx.service - A high performance web server and a reverse proxy server
     Loaded: loaded (/lib/systemd/system/nginx.service; enabled; vendor preset: enabled)
     Active: active (running) since Mon 2024-01-29 10:20:11 UTC; 2min 57s ago
       Docs: man:nginx(8)
    Process: 2090 ExecStartPre=/usr/sbin/nginx -t -q -g daemon on; master_process on; (code=exited, status=0/SUCCESS)
    Process: 2097 ExecStart=/usr/sbin/nginx -g daemon on; master_process on; (code=exited, status=0/SUCCESS)
   Main PID: 2205 (nginx)
      Tasks: 2 (limit: 1121)
     Memory: 4.3M
        CPU: 25ms
     CGroup: /system.slice/nginx.service
             ├─2205 "nginx: master process /usr/sbin/nginx -g daemon on; master_process on;"
             └─2208 "nginx: worker process" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "" "" ""

Jan 29 10:20:11 ip-172-31-23-206 systemd[1]: Starting A high performance web server and a reverse proxy server...
Jan 29 10:20:11 ip-172-31-23-206 systemd[1]: Started A high performance web server and a reverse proxy server.
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
lines 1-16/16 (END)

# Test cebserver connectivity here
ubuntu@ip-172-31-23-206:~$ `curl http:// 127.0.0.1:80`
curl: (3) URL using bad/illegal format or missing URL
<!DOCTYPE html>
<html>
<head>
<title>Welcome to nginx!</title>
<style>
    body {
        width: 35em;
        margin: 0 auto;
        font-family: Tahoma, Verdana, Arial, sans-serif;
    }
</style>
</head>
<body>
<h1>Welcome to nginx!</h1>
<p>If you see this page, the nginx web server is successfully installed and
working. Further configuration is required.</p>

<p>For online documentation and support please refer to
<a href="http://nginx.org/">nginx.org</a>.<br/>
Commercial support is available at
<a href="http://nginx.com/">nginx.com</a>.</p>

<p><em>Thank you for using nginx.</em></p>
</body>
</html>
ubuntu@ip-172-31-23-206:~$ `curl -s http://169.254.169.254/latest/meta-data/public-ipv4`
<?xml version="1.0" encoding="iso-8859-1"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
        "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
 <head>
  <title>401 - Unauthorized</title>
 </head>
 <body>
  <h1>401 - Unauthorized</h1>
 </body>
</html>
## Activate the http security protocol for the EC2 instance with port 80 Query with http://your.ip:80

![Acivate port 80](prjct_img/nginx_http.JPG)

ubuntu@ip-172-31-23-206:~$ sudo apt install mysql-server
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  libcgi-fast-perl libcgi-pm-perl libclone-perl libencode-locale-perl libevent-pthreads-2.1-7 libfcgi-bin libfcgi-perl libfcgi0ldbl libhtml-parser-perl libhtml-tagset-perl libhtml-template-per
  libhttp-date-perl libhttp-message-perl libio-html-perl liblwp-mediatypes-perl libmecab2 libprotobuf-lite23 libtimedate-perl liburi-perl mecab-ipadic mecab-ipadic-utf8 mecab-utils mysql-clien
  mysql-client-core-8.0 mysql-common mysql-server-8.0 mysql-server-core-8.0
Suggested packages:
  libdata-dump-perl libipc-sharedcache-perl libbusiness-isbn-perl libwww-perl mailx tinyca
The following NEW packages will be installed:
  libcgi-fast-perl libcgi-pm-perl libclone-perl libencode-locale-perl libevent-pthreads-2.1-7 libfcgi-bin libfcgi-perl libfcgi0ldbl libhtml-parser-perl libhtml-tagset-perl libhtml-template-per
  libhttp-date-perl libhttp-message-perl libio-html-perl liblwp-mediatypes-perl libmecab2 libprotobuf-lite23 libtimedate-perl liburi-perl mecab-ipadic mecab-ipadic-utf8 mecab-utils mysql-clien
  mysql-client-core-8.0 mysql-common mysql-server mysql-server-8.0 mysql-server-core-8.0
0 upgraded, 28 newly installed, 0 to remove and 57 not upgraded.
Need to get 29.6 MB of archives.
After this operation, 243 MB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 mysql-common all 5.8+1.0.8 [7212 B]
Get:2 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 mysql-client-core-8.0 amd64 8.0.35-0ubuntu0.22.04.1 [2682 kB]
Get:3 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 mysql-client-8.0 amd64 8.0.35-0ubuntu0.22.04.1 [22.7 kB]
Get:4 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libevent-pthreads-2.1-7 amd64 2.1.12-stable-1build3 [7642 B]
Get:5 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libmecab2 amd64 0.996-14build9 [199 kB]
Get:6 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 libprotobuf-lite23 amd64 3.12.4-1ubuntu7.22.04.1 [209 kB]
Get:7 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 mysql-server-core-8.0 amd64 8.0.35-0ubuntu0.22.04.1 [17.6 MB]
Get:8 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 mysql-server-8.0 amd64 8.0.35-0ubuntu0.22.04.1 [1438 kB]
Get:9 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libhtml-tagset-perl all 3.20-4 [12.5 kB]
Get:10 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 liburi-perl all 5.10-1 [78.8 kB]
Get:11 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libhtml-parser-perl amd64 3.76-1build2 [88.4 kB]
Get:12 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libcgi-pm-perl all 4.54-1 [188 kB]
Get:13 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libfcgi0ldbl amd64 2.4.2-2build2 [28.0 kB]
Get:14 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libfcgi-perl amd64 0.82+ds-1build1 [22.8 kB]
Get:15 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libcgi-fast-perl all 1:2.15-1 [10.5 kB]
Get:16 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libclone-perl amd64 0.45-1build3 [11.0 kB]
Get:17 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libencode-locale-perl all 1.05-1.1 [11.8 kB]
Get:18 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libfcgi-bin amd64 2.4.2-2build2 [11.2 kB]
Get:19 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libhtml-template-perl all 2.97-1.1 [59.1 kB]
Get:20 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libtimedate-perl all 2.3300-2 [34.0 kB]
Get:21 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libhttp-date-perl all 6.05-1 [9920 B]
Get:22 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libio-html-perl all 1.004-2 [15.4 kB]
Get:23 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 liblwp-mediatypes-perl all 6.04-1 [19.5 kB]
Get:24 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 libhttp-message-perl all 6.36-1 [76.8 kB]
Get:25 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 mecab-utils amd64 0.996-14build9 [4850 B]
Get:26 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 mecab-ipadic all 2.7.0-20070801+main-3 [6718 kB]
Get:27 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 mecab-ipadic-utf8 all 2.7.0-20070801+main-3 [4384 B]
Get:28 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 mysql-server all 8.0.35-0ubuntu0.22.04.1 [9464 B]
Fetched 29.6 MB in 1s (48.1 MB/s)
Preconfiguring packages ...
Selecting previously unselected package mysql-common.
(Reading database ... 65041 files and directories currently installed.)
Preparing to unpack .../0-mysql-common_5.8+1.0.8_all.deb ...
Unpacking mysql-common (5.8+1.0.8) ...
Selecting previously unselected package mysql-client-core-8.0.
Preparing to unpack .../1-mysql-client-core-8.0_8.0.35-0ubuntu0.22.04.1_amd64.deb ...
Unpacking mysql-client-core-8.0 (8.0.35-0ubuntu0.22.04.1) ...
Selecting previously unselected package mysql-client-8.0.
Preparing to unpack .../2-mysql-client-8.0_8.0.35-0ubuntu0.22.04.1_amd64.deb ...
Unpacking mysql-client-8.0 (8.0.35-0ubuntu0.22.04.1) ...
Selecting previously unselected package libevent-pthreads-2.1-7:amd64.
Preparing to unpack .../3-libevent-pthreads-2.1-7_2.1.12-stable-1build3_amd64.deb ...
Unpacking libevent-pthreads-2.1-7:amd64 (2.1.12-stable-1build3) ...
Selecting previously unselected package libmecab2:amd64.
Preparing to unpack .../4-libmecab2_0.996-14build9_amd64.deb ...
Unpacking libmecab2:amd64 (0.996-14build9) ...
Selecting previously unselected package libprotobuf-lite23:amd64.
Preparing to unpack .../5-libprotobuf-lite23_3.12.4-1ubuntu7.22.04.1_amd64.deb ...
Unpacking libprotobuf-lite23:amd64 (3.12.4-1ubuntu7.22.04.1) ...
Selecting previously unselected package mysql-server-core-8.0.
Preparing to unpack .../6-mysql-server-core-8.0_8.0.35-0ubuntu0.22.04.1_amd64.deb ...
Unpacking mysql-server-core-8.0 (8.0.35-0ubuntu0.22.04.1) ...
Setting up mysql-common (5.8+1.0.8) ...
update-alternatives: using /etc/mysql/my.cnf.fallback to provide /etc/mysql/my.cnf (my.cnf) in auto mode
Selecting previously unselected package mysql-server-8.0.
(Reading database ... 65255 files and directories currently installed.)
Preparing to unpack .../00-mysql-server-8.0_8.0.35-0ubuntu0.22.04.1_amd64.deb ...
Unpacking mysql-server-8.0 (8.0.35-0ubuntu0.22.04.1) ...
Selecting previously unselected package libhtml-tagset-perl.
Preparing to unpack .../01-libhtml-tagset-perl_3.20-4_all.deb ...
Unpacking libhtml-tagset-perl (3.20-4) ...
Selecting previously unselected package liburi-perl.
Preparing to unpack .../02-liburi-perl_5.10-1_all.deb ...
Unpacking liburi-perl (5.10-1) ...
Selecting previously unselected package libhtml-parser-perl:amd64.
Preparing to unpack .../03-libhtml-parser-perl_3.76-1build2_amd64.deb ...
Unpacking libhtml-parser-perl:amd64 (3.76-1build2) ...
Selecting previously unselected package libcgi-pm-perl.
Preparing to unpack .../04-libcgi-pm-perl_4.54-1_all.deb ...
Unpacking libcgi-pm-perl (4.54-1) ...
Selecting previously unselected package libfcgi0ldbl:amd64.
Preparing to unpack .../05-libfcgi0ldbl_2.4.2-2build2_amd64.deb ...
Unpacking libfcgi0ldbl:amd64 (2.4.2-2build2) ...
Selecting previously unselected package libfcgi-perl:amd64.
Preparing to unpack .../06-libfcgi-perl_0.82+ds-1build1_amd64.deb ...
Unpacking libfcgi-perl:amd64 (0.82+ds-1build1) ...
Selecting previously unselected package libcgi-fast-perl.
Preparing to unpack .../07-libcgi-fast-perl_1%3a2.15-1_all.deb ...
Unpacking libcgi-fast-perl (1:2.15-1) ...
Selecting previously unselected package libclone-perl.
Preparing to unpack .../08-libclone-perl_0.45-1build3_amd64.deb ...
Unpacking libclone-perl (0.45-1build3) ...
Selecting previously unselected package libencode-locale-perl.
Preparing to unpack .../09-libencode-locale-perl_1.05-1.1_all.deb ...
Unpacking libencode-locale-perl (1.05-1.1) ...
Selecting previously unselected package libfcgi-bin.
Preparing to unpack .../10-libfcgi-bin_2.4.2-2build2_amd64.deb ...
Unpacking libfcgi-bin (2.4.2-2build2) ...
Selecting previously unselected package libhtml-template-perl.
Preparing to unpack .../11-libhtml-template-perl_2.97-1.1_all.deb ...
Unpacking libhtml-template-perl (2.97-1.1) ...
Selecting previously unselected package libtimedate-perl.
Preparing to unpack .../12-libtimedate-perl_2.3300-2_all.deb ...
Unpacking libtimedate-perl (2.3300-2) ...
Selecting previously unselected package libhttp-date-perl.
Preparing to unpack .../13-libhttp-date-perl_6.05-1_all.deb ...
Unpacking libhttp-date-perl (6.05-1) ...
Selecting previously unselected package libio-html-perl.
Preparing to unpack .../14-libio-html-perl_1.004-2_all.deb ...
Unpacking libio-html-perl (1.004-2) ...
Selecting previously unselected package liblwp-mediatypes-perl.
Preparing to unpack .../15-liblwp-mediatypes-perl_6.04-1_all.deb ...
Unpacking liblwp-mediatypes-perl (6.04-1) ...
Selecting previously unselected package libhttp-message-perl.
Preparing to unpack .../16-libhttp-message-perl_6.36-1_all.deb ...
Unpacking libhttp-message-perl (6.36-1) ...
Selecting previously unselected package mecab-utils.
Preparing to unpack .../17-mecab-utils_0.996-14build9_amd64.deb ...
Unpacking mecab-utils (0.996-14build9) ...
Selecting previously unselected package mecab-ipadic.
Preparing to unpack .../18-mecab-ipadic_2.7.0-20070801+main-3_all.deb ...
Unpacking mecab-ipadic (2.7.0-20070801+main-3) ...
Selecting previously unselected package mecab-ipadic-utf8.
Preparing to unpack .../19-mecab-ipadic-utf8_2.7.0-20070801+main-3_all.deb ...
Unpacking mecab-ipadic-utf8 (2.7.0-20070801+main-3) ...
Selecting previously unselected package mysql-server.
Preparing to unpack .../20-mysql-server_8.0.35-0ubuntu0.22.04.1_all.deb ...
Unpacking mysql-server (8.0.35-0ubuntu0.22.04.1) ...
Setting up libmecab2:amd64 (0.996-14build9) ...
Setting up mysql-client-core-8.0 (8.0.35-0ubuntu0.22.04.1) ...
Setting up libfcgi0ldbl:amd64 (2.4.2-2build2) ...
Setting up libclone-perl (0.45-1build3) ...
Setting up libhtml-tagset-perl (3.20-4) ...
Setting up liblwp-mediatypes-perl (6.04-1) ...
Setting up libfcgi-bin (2.4.2-2build2) ...
Setting up libencode-locale-perl (1.05-1.1) ...
Setting up libprotobuf-lite23:amd64 (3.12.4-1ubuntu7.22.04.1) ...
Setting up mecab-utils (0.996-14build9) ...
Setting up libio-html-perl (1.004-2) ...
Setting up libtimedate-perl (2.3300-2) ...
Setting up mysql-client-8.0 (8.0.35-0ubuntu0.22.04.1) ...
Setting up libfcgi-perl:amd64 (0.82+ds-1build1) ...
Setting up liburi-perl (5.10-1) ...
Setting up libevent-pthreads-2.1-7:amd64 (2.1.12-stable-1build3) ...
Setting up libhttp-date-perl (6.05-1) ...
Setting up mecab-ipadic (2.7.0-20070801+main-3) ...
Compiling IPA dictionary for Mecab.  This takes long time...
reading /usr/share/mecab/dic/ipadic/unk.def ... 40
emitting double-array: 100% |###########################################|
/usr/share/mecab/dic/ipadic/model.def is not found. skipped.
reading /usr/share/mecab/dic/ipadic/Interjection.csv ... 252
reading /usr/share/mecab/dic/ipadic/Suffix.csv ... 1393
reading /usr/share/mecab/dic/ipadic/Noun.adjv.csv ... 3328
reading /usr/share/mecab/dic/ipadic/Noun.verbal.csv ... 12146
reading /usr/share/mecab/dic/ipadic/Verb.csv ... 130750
reading /usr/share/mecab/dic/ipadic/Prefix.csv ... 221
reading /usr/share/mecab/dic/ipadic/Noun.number.csv ... 42
reading /usr/share/mecab/dic/ipadic/Postp.csv ... 146
reading /usr/share/mecab/dic/ipadic/Adverb.csv ... 3032
reading /usr/share/mecab/dic/ipadic/Others.csv ... 2
reading /usr/share/mecab/dic/ipadic/Noun.demonst.csv ... 120
reading /usr/share/mecab/dic/ipadic/Noun.nai.csv ... 42
reading /usr/share/mecab/dic/ipadic/Noun.csv ... 60477
reading /usr/share/mecab/dic/ipadic/Adnominal.csv ... 135
reading /usr/share/mecab/dic/ipadic/Noun.place.csv ... 72999
reading /usr/share/mecab/dic/ipadic/Conjunction.csv ... 171
reading /usr/share/mecab/dic/ipadic/Filler.csv ... 19
reading /usr/share/mecab/dic/ipadic/Auxil.csv ... 199
reading /usr/share/mecab/dic/ipadic/Postp-col.csv ... 91
reading /usr/share/mecab/dic/ipadic/Symbol.csv ... 208
reading /usr/share/mecab/dic/ipadic/Adj.csv ... 27210
reading /usr/share/mecab/dic/ipadic/Noun.others.csv ... 151
reading /usr/share/mecab/dic/ipadic/Noun.name.csv ... 34202
reading /usr/share/mecab/dic/ipadic/Noun.org.csv ... 16668
reading /usr/share/mecab/dic/ipadic/Noun.proper.csv ... 27328
reading /usr/share/mecab/dic/ipadic/Noun.adverbal.csv ... 795
emitting double-array: 100% |###########################################|
reading /usr/share/mecab/dic/ipadic/matrix.def ... 1316x1316
emitting matrix      : 100% |###########################################|

done!
update-alternatives: using /var/lib/mecab/dic/ipadic to provide /var/lib/mecab/dic/debian (mecab-dictionary) in auto mode
Setting up mysql-server-core-8.0 (8.0.35-0ubuntu0.22.04.1) ...
Setting up mecab-ipadic-utf8 (2.7.0-20070801+main-3) ...
Compiling IPA dictionary for Mecab.  This takes long time...
reading /usr/share/mecab/dic/ipadic/unk.def ... 40
emitting double-array: 100% |###########################################|
/usr/share/mecab/dic/ipadic/model.def is not found. skipped.
reading /usr/share/mecab/dic/ipadic/Interjection.csv ... 252
reading /usr/share/mecab/dic/ipadic/Suffix.csv ... 1393
reading /usr/share/mecab/dic/ipadic/Noun.adjv.csv ... 3328
reading /usr/share/mecab/dic/ipadic/Noun.verbal.csv ... 12146
reading /usr/share/mecab/dic/ipadic/Verb.csv ... 130750
reading /usr/share/mecab/dic/ipadic/Prefix.csv ... 221
reading /usr/share/mecab/dic/ipadic/Noun.number.csv ... 42
reading /usr/share/mecab/dic/ipadic/Postp.csv ... 146
reading /usr/share/mecab/dic/ipadic/Adverb.csv ... 3032
reading /usr/share/mecab/dic/ipadic/Others.csv ... 2
reading /usr/share/mecab/dic/ipadic/Noun.demonst.csv ... 120
reading /usr/share/mecab/dic/ipadic/Noun.nai.csv ... 42
reading /usr/share/mecab/dic/ipadic/Noun.csv ... 60477
reading /usr/share/mecab/dic/ipadic/Adnominal.csv ... 135
reading /usr/share/mecab/dic/ipadic/Noun.place.csv ... 72999
reading /usr/share/mecab/dic/ipadic/Conjunction.csv ... 171
reading /usr/share/mecab/dic/ipadic/Filler.csv ... 19
reading /usr/share/mecab/dic/ipadic/Auxil.csv ... 199
reading /usr/share/mecab/dic/ipadic/Postp-col.csv ... 91
reading /usr/share/mecab/dic/ipadic/Symbol.csv ... 208
reading /usr/share/mecab/dic/ipadic/Adj.csv ... 27210
reading /usr/share/mecab/dic/ipadic/Noun.others.csv ... 151
reading /usr/share/mecab/dic/ipadic/Noun.name.csv ... 34202
reading /usr/share/mecab/dic/ipadic/Noun.org.csv ... 16668
reading /usr/share/mecab/dic/ipadic/Noun.proper.csv ... 27328
reading /usr/share/mecab/dic/ipadic/Noun.adverbal.csv ... 795
emitting double-array: 100% |###########################################|
reading /usr/share/mecab/dic/ipadic/matrix.def ... 1316x1316
emitting matrix      : 100% |###########################################|

done!
update-alternatives: using /var/lib/mecab/dic/ipadic-utf8 to provide /var/lib/mecab/dic/debian (mecab-dictionary) in auto mode
Setting up libhtml-parser-perl:amd64 (3.76-1build2) ...
Setting up libhttp-message-perl (6.36-1) ...
Setting up mysql-server-8.0 (8.0.35-0ubuntu0.22.04.1) ...
update-alternatives: using /etc/mysql/mysql.cnf to provide /etc/mysql/my.cnf (my.cnf) in auto mode
Renaming removed key_buffer and myisam-recover options (if present)
mysqld will log errors to /var/log/mysql/error.log
mysqld is running as pid 2847
Created symlink /etc/systemd/system/multi-user.target.wants/mysql.service → /lib/systemd/system/mysql.service.
Setting up libcgi-pm-perl (4.54-1) ...
Setting up libhtml-template-perl (2.97-1.1) ...
Setting up mysql-server (8.0.35-0ubuntu0.22.04.1) ...
Setting up libcgi-fast-perl (1:2.15-1) ...
Processing triggers for man-db (2.10.2-1) ...
Processing triggers for libc-bin (2.35-0ubuntu3.4) ...
Scanning processes...
Scanning linux images...

Running kernel seems to be up-to-date.

No services need to be restarted.

No containers need to be restarted.

No user sessions are running outdated binaries.

No VM guests are running outdated hypervisor (qemu) binaries on this host.
ubuntu@ip-172-31-23-206:~$ sudo mysql
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 8
Server version: 8.0.35-0ubuntu0.22.04.1 (Ubuntu)

Copyright (c) 2000, 2023, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> ALTER USER  'root'@'localhost' IDENTIFIED with mysql_native_password BY "B3tt3rthanvs!x"
    -> ;
Query OK, 0 rows affected (0.02 sec)

mysql> exit
Bye
ubuntu@ip-172-31-23-206:~$ sudo mysql_secure_installation

Securing the MySQL server deployment.

Enter password for user root:

VALIDATE PASSWORD COMPONENT can be used to test passwords
and improve security. It checks the strength of password
and allows the users to set only those passwords which are
secure enough. Would you like to setup VALIDATE PASSWORD component?

Press y|Y for Yes, any other key for No: ^Y
Using existing password for root.
Change the password for root ? ((Press y|Y for Yes, any other key for No) : g

 ... skipping.
By default, a MySQL installation has an anonymous user,
allowing anyone to log into MySQL without having to have
a user account created for them. This is intended only for
testing, and to make the installation go a bit smoother.
You should remove them before moving into a production
environment.

Remove anonymous users? (Press y|Y for Yes, any other key for No) : n

 ... skipping.


Normally, root should only be allowed to connect from
'localhost'. This ensures that someone cannot guess at
the root password from the network.

Disallow root login remotely? (Press y|Y for Yes, any other key for No) : f

 ... skipping.
By default, MySQL comes with a database named 'test' that
anyone can access. This is also intended only for testing,
and should be removed before moving into a production
environment.


Remove test database and access to it? (Press y|Y for Yes, any other key for No) : h

 ... skipping.
Reloading the privilege tables will ensure that all changes
made so far will take effect immediately.

Reload privilege tables now? (Press y|Y for Yes, any other key for No) : d

 ... skipping.
All done!
ubuntu@ip-172-31-23-206:~$ client_loop: send disconnect: Connection reset by peer

CLS-PC@NEW-ANPN1N9QSNR MINGW64 ~
$ ssh -i pbl2.pem ubuntu@ec2-34-211-170-9.us-west-2.compute.amazonaws.com
Welcome to Ubuntu 22.04.3 LTS (GNU/Linux 6.2.0-1017-aws x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

  System information as of Mon Jan 29 13:36:56 UTC 2024

  System load:  0.0               Processes:             101
  Usage of /:   30.0% of 7.57GB   Users logged in:       0
  Memory usage: 59%               IPv4 address for eth0: 172.31.23.206
  Swap usage:   0%

 * Ubuntu Pro delivers the most comprehensive open source security and
   compliance features.

   https://ubuntu.com/aws/pro

Expanded Security Maintenance for Applications is not enabled.

61 updates can be applied immediately.
34 of these updates are standard security updates.
To see these additional updates run: apt list --upgradable

Enable ESM Apps to receive additional future security updates.
See https://ubuntu.com/esm or run: sudo pro status


Last login: Mon Jan 29 10:17:11 2024 from 102.211.164.2
ubuntu@ip-172-31-23-206:~$ $ sudo apt install php-fpm php-mysql
$: command not found
ubuntu@ip-172-31-23-206:~$ sudo apt install php-fpm php-mysql
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  bzip2 mailcap mime-support php-common php8.1-cli php8.1-common php8.1-fpm php8.1-mysql php8.1-opcache php8.1-readline
Suggested packages:
  bzip2-doc php-pear
The following NEW packages will be installed:
  bzip2 mailcap mime-support php-common php-fpm php-mysql php8.1-cli php8.1-common php8.1-fpm php8.1-mysql php8.1-opcache php8.1-readline
0 upgraded, 12 newly installed, 0 to remove and 57 not upgraded.
Need to get 5389 kB of archives.
After this operation, 22.2 MB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 bzip2 amd64 1.0.8-5build1 [34.8 kB]
Get:2 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 mailcap all 3.70+nmu1ubuntu1 [23.8 kB]
Get:3 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 mime-support all 3.66 [3696 B]
Get:4 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 php-common all 2:92ubuntu1 [12.4 kB]
Get:5 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 php8.1-common amd64 8.1.2-1ubuntu2.14 [1127 kB]
Get:6 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 php8.1-opcache amd64 8.1.2-1ubuntu2.14 [365 kB]
Get:7 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 php8.1-readline amd64 8.1.2-1ubuntu2.14 [13.6 kB]
Get:8 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 php8.1-cli amd64 8.1.2-1ubuntu2.14 [1834 kB]
Get:9 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/universe amd64 php8.1-fpm amd64 8.1.2-1ubuntu2.14 [1840 kB]
Get:10 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/universe amd64 php-fpm all 2:8.1+92ubuntu1 [2838 B]
Get:11 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy-updates/main amd64 php8.1-mysql amd64 8.1.2-1ubuntu2.14 [130 kB]
Get:12 http://us-west-2.ec2.archive.ubuntu.com/ubuntu jammy/main amd64 php-mysql all 2:8.1+92ubuntu1 [1834 B]
Fetched 5389 kB in 0s (44.3 MB/s)
Selecting previously unselected package bzip2.
(Reading database ... 65643 files and directories currently installed.)
Preparing to unpack .../00-bzip2_1.0.8-5build1_amd64.deb ...
Unpacking bzip2 (1.0.8-5build1) ...
Selecting previously unselected package mailcap.
Preparing to unpack .../01-mailcap_3.70+nmu1ubuntu1_all.deb ...
Unpacking mailcap (3.70+nmu1ubuntu1) ...
Selecting previously unselected package mime-support.
Preparing to unpack .../02-mime-support_3.66_all.deb ...
Unpacking mime-support (3.66) ...
Selecting previously unselected package php-common.
Preparing to unpack .../03-php-common_2%3a92ubuntu1_all.deb ...
Unpacking php-common (2:92ubuntu1) ...
Selecting previously unselected package php8.1-common.
Preparing to unpack .../04-php8.1-common_8.1.2-1ubuntu2.14_amd64.deb ...
Unpacking php8.1-common (8.1.2-1ubuntu2.14) ...
Selecting previously unselected package php8.1-opcache.
Preparing to unpack .../05-php8.1-opcache_8.1.2-1ubuntu2.14_amd64.deb ...
Unpacking php8.1-opcache (8.1.2-1ubuntu2.14) ...
Selecting previously unselected package php8.1-readline.
Preparing to unpack .../06-php8.1-readline_8.1.2-1ubuntu2.14_amd64.deb ...
Unpacking php8.1-readline (8.1.2-1ubuntu2.14) ...
Selecting previously unselected package php8.1-cli.
Preparing to unpack .../07-php8.1-cli_8.1.2-1ubuntu2.14_amd64.deb ...
Unpacking php8.1-cli (8.1.2-1ubuntu2.14) ...
Selecting previously unselected package php8.1-fpm.
Preparing to unpack .../08-php8.1-fpm_8.1.2-1ubuntu2.14_amd64.deb ...
Unpacking php8.1-fpm (8.1.2-1ubuntu2.14) ...
Selecting previously unselected package php-fpm.
Preparing to unpack .../09-php-fpm_2%3a8.1+92ubuntu1_all.deb ...
Unpacking php-fpm (2:8.1+92ubuntu1) ...
Selecting previously unselected package php8.1-mysql.
Preparing to unpack .../10-php8.1-mysql_8.1.2-1ubuntu2.14_amd64.deb ...
Unpacking php8.1-mysql (8.1.2-1ubuntu2.14) ...
Selecting previously unselected package php-mysql.
Preparing to unpack .../11-php-mysql_2%3a8.1+92ubuntu1_all.deb ...
Unpacking php-mysql (2:8.1+92ubuntu1) ...
Setting up php-common (2:92ubuntu1) ...
Created symlink /etc/systemd/system/timers.target.wants/phpsessionclean.timer → /lib/systemd/system/phpsessionclean.timer.
Setting up php8.1-common (8.1.2-1ubuntu2.14) ...

Creating config file /etc/php/8.1/mods-available/calendar.ini with new version

Creating config file /etc/php/8.1/mods-available/ctype.ini with new version

Creating config file /etc/php/8.1/mods-available/exif.ini with new version

Creating config file /etc/php/8.1/mods-available/fileinfo.ini with new version

Creating config file /etc/php/8.1/mods-available/ffi.ini with new version

Creating config file /etc/php/8.1/mods-available/ftp.ini with new version

Creating config file /etc/php/8.1/mods-available/gettext.ini with new version

Creating config file /etc/php/8.1/mods-available/iconv.ini with new version

Creating config file /etc/php/8.1/mods-available/pdo.ini with new version

Creating config file /etc/php/8.1/mods-available/phar.ini with new version

Creating config file /etc/php/8.1/mods-available/posix.ini with new version

Creating config file /etc/php/8.1/mods-available/shmop.ini with new version

Creating config file /etc/php/8.1/mods-available/sockets.ini with new version

Creating config file /etc/php/8.1/mods-available/sysvmsg.ini with new version

Creating config file /etc/php/8.1/mods-available/sysvsem.ini with new version

Creating config file /etc/php/8.1/mods-available/sysvshm.ini with new version

Creating config file /etc/php/8.1/mods-available/tokenizer.ini with new version
Setting up bzip2 (1.0.8-5build1) ...
Setting up php8.1-mysql (8.1.2-1ubuntu2.14) ...

Creating config file /etc/php/8.1/mods-available/mysqlnd.ini with new version

Creating config file /etc/php/8.1/mods-available/mysqli.ini with new version

Creating config file /etc/php/8.1/mods-available/pdo_mysql.ini with new version
Setting up php8.1-readline (8.1.2-1ubuntu2.14) ...

Creating config file /etc/php/8.1/mods-available/readline.ini with new version
Setting up mailcap (3.70+nmu1ubuntu1) ...
Setting up php8.1-opcache (8.1.2-1ubuntu2.14) ...

Creating config file /etc/php/8.1/mods-available/opcache.ini with new version
Setting up php-mysql (2:8.1+92ubuntu1) ...
Setting up mime-support (3.66) ...
Setting up php8.1-cli (8.1.2-1ubuntu2.14) ...
update-alternatives: using /usr/bin/php8.1 to provide /usr/bin/php (php) in auto mode
update-alternatives: using /usr/bin/phar8.1 to provide /usr/bin/phar (phar) in auto mode
update-alternatives: using /usr/bin/phar.phar8.1 to provide /usr/bin/phar.phar (phar.phar) in auto mode

Creating config file /etc/php/8.1/cli/php.ini with new version
Setting up php8.1-fpm (8.1.2-1ubuntu2.14) ...

Creating config file /etc/php/8.1/fpm/php.ini with new version
Created symlink /etc/systemd/system/multi-user.target.wants/php8.1-fpm.service → /lib/systemd/system/php8.1-fpm.service.
Setting up php-fpm (2:8.1+92ubuntu1) ...
Processing triggers for man-db (2.10.2-1) ...
Processing triggers for php8.1-cli (8.1.2-1ubuntu2.14) ...
Processing triggers for php8.1-fpm (8.1.2-1ubuntu2.14) ...
Scanning processes...
Scanning linux images...

Running kernel seems to be up-to-date.

No services need to be restarted.

No containers need to be restarted.

No user sessions are running outdated binaries.

No VM guests are running outdated hypervisor (qemu) binaries on this host.
ubuntu@ip-172-31-23-206:~$ client_loop: send disconnect: Connection reset by peer

CLS-PC@NEW-ANPN1N9QSNR MINGW64 ~
$ ssh -i pbl2.pem ubuntu@ec2-34-211-170-9.us-west-2.compute.amazonaws.com
Welcome to Ubuntu 22.04.3 LTS (GNU/Linux 6.2.0-1017-aws x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

  System information as of Mon Jan 29 14:24:43 UTC 2024

  System load:  0.0               Processes:             104
  Usage of /:   30.3% of 7.57GB   Users logged in:       1
  Memory usage: 60%               IPv4 address for eth0: 172.31.23.206
  Swap usage:   0%

 * Ubuntu Pro delivers the most comprehensive open source security and
   compliance features.

   https://ubuntu.com/aws/pro

Expanded Security Maintenance for Applications is not enabled.

61 updates can be applied immediately.
34 of these updates are standard security updates.
To see these additional updates run: apt list --upgradable

Enable ESM Apps to receive additional future security updates.
See https://ubuntu.com/esm or run: sudo pro status


Last login: Mon Jan 29 13:36:57 2024 from 102.211.164.2
ubuntu@ip-172-31-23-206:~$ $ sudo mkdir /var/www/projectLEMP
$: command not found
ubuntu@ip-172-31-23-206:~$ sudo mkdir /var/www/projectLEMP
ubuntu@ip-172-31-23-206:~$ sudo own $USER:$USER /var/www/projectLEMP
sudo: own: command not found
ubuntu@ip-172-31-23-206:~$ sudo chown $USER:$USER /var/www/projectLEMP
ubuntu@ip-172-31-23-206:~$ sudo nano /etc/nginx/sites-available/projectLEMP
ubuntu@ip-172-31-23-206:~$ sudo ln -s /etc/nginx/sites-available/projectLEMP /etc/nginx/sites-enabled/
ubuntu@ip-172-31-23-206:~$ sudo nginx -t
nginx: the configuration file /etc/nginx/nginx.conf syntax is ok
nginx: configuration file /etc/nginx/nginx.conf test is successful
ubuntu@ip-172-31-23-206:~$ sudo unlink /etc/nginx/sites-enabled/default
ubuntu@ip-172-31-23-206:~$ sudo systemctl reload nginx
ubuntu@ip-172-31-23-206:~$ sudo echo 'Hello LEMP from hostname' $(curl -s http://169.254.169.254/latest/meta-data/public-hostname) 'with public IP' $(curl -s http://169.254.169.254/latest/meta-data/public-ipv4) > /var/www/projectLEMP/index.html
ubuntu@ip-172-31-23-206:~$ nano /var/www/projectLEMP/info.php
ubuntu@ip-172-31-23-206:~$ sudo mysql
ERROR 1045 (28000): Access denied for user 'root'@'localhost' (using password: NO)
ubuntu@ip-172-31-23-206:~$ sudo mysql -p
Enter password:
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 12
Server version: 8.0.35-0ubuntu0.22.04.1 (Ubuntu)

Copyright (c) 2000, 2023, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> mysql> CREATE DATABASE `example_database`;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'mysql> CREATE DATABASE `example_database`' at line 1
mysql> CREATE DATABASE `example_database`;
Query OK, 1 row affected (0.07 sec)

mysql> CREATE USER 'coffeedcognac'@'%' IDENTIFIED WITH mysql_native_password BY 'PassWord.2';
Query OK, 0 rows affected (0.03 sec)

mysql> GRANT ALL ON example_database.* TO 'coffeedcognac'@'%';
Query OK, 0 rows affected (0.01 sec)

mysql> exit
Bye
ubuntu@ip-172-31-23-206:~$ mysql -u coffeedcognac -p
Enter password:
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 13
Server version: 8.0.35-0ubuntu0.22.04.1 (Ubuntu)

Copyright (c) 2000, 2023, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> SHOW DATABASES;
+--------------------+
| Database           |
+--------------------+
| example_database   |
| information_schema |
| performance_schema |
+--------------------+
3 rows in set (0.02 sec)

mysql> CREATE TABLE example_database.todo_list (item_id INT AUTO_INCREMENT,content VARCHAR(255),PRIMARY KEY(item_id));
Query OK, 0 rows affected (0.04 sec)

mysql> INSERT INTO example_database.todo_list (content) VALUES ("I am doing laundry today");
Query OK, 1 row affected (0.04 sec)

mysql> SELECT * FROM example_database.todo_list;
+---------+--------------------------+
| item_id | content                  |
+---------+--------------------------+
|       1 | I am doing laundry today |
+---------+--------------------------+
1 row in set (0.00 sec)

mysql> -- Inserting multiple tasks into the todo_list table
mysql> INSERT INTO example_database.todo_list (content) VALUES
    -> ("I am doing laundry today"),
    -> ("Buy groceries for the week"),
    -> ("Prepare for the meeting tomorrow"),
    -> ("Go for a run in the evening");
Query OK, 4 rows affected (0.01 sec)
Records: 4  Duplicates: 0  Warnings: 0

mysql> -- Deleting a specific task from the todo_list table
mysql> DELETE FROM example_database.todo_list WHERE content = "I am doing laundry today";
Query OK, 2 rows affected (0.01 sec)

mysql> INSERT INTO example_database.todo_list (content) VALUES ("I am doing laundry today");
Query OK, 1 row affected (0.00 sec)

mysql> SELECT * FROM example_database.todo_list;
+---------+----------------------------------+
| item_id | content                          |
+---------+----------------------------------+
|       3 | Buy groceries for the week       |
|       4 | Prepare for the meeting tomorrow |
|       5 | Go for a run in the evening      |
|       6 | I am doing laundry today         |
+---------+----------------------------------+
4 rows in set (0.00 sec)

mysql> exit
Bye
ubuntu@ip-172-31-23-206:~$ nano /var/www/projectLEMP/todo_list.php
ubuntu@ip-172-31-23-206:~$ nano /var/www/projectLEMP/todo_list.php
