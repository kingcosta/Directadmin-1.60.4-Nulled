# Directadmin-1.60.4-Nulled
Directadmin 1.60.4 Nulled + Working License File ( Unlimited Account, Unlimited Domains )


[root@sucuri ~]# yum -y install nano wget perl

[root@sucuri ~]# wget https://raw.githubusercontent.com/LinuxGuard/Directadmin-1.60.4-Nulled/master/setup.sh

[root@sucuri ~]# chmod +x setup.sh

[root@sucuri ~]# ./setup.sh

Client ID (uid):  9192
License ID (lid): 919233

[root@sucuri ~]# firewall-cmd --zone=public --add-port=21/tcp --permanent

[root@sucuri ~]# firewall-cmd --zone=public --add-port=22/tcp --permanent

[root@sucuri ~]# firewall-cmd --zone=public --add-port=25/tcp --permanent

[root@sucuri ~]# firewall-cmd --zone=public --add-port=80/tcp --permanent

[root@sucuri ~]# firewall-cmd --zone=public --add-port=443/tcp --permanent

[root@sucuri ~]# firewall-cmd --zone=public --add-port=465/tcp --permanent

[root@sucuri ~]# firewall-cmd --zone=public --add-port=2222/tcp --permanent

[root@sucuri ~]# firewall-cmd --reload

[root@sucuri ~]# systemctl restart directadmin

[root@sucuri ~]# cd /usr/local/directadmin/conf/

[root@sucuri ~]# systemctl stop directadmin

[root@sucuri ~]# rm -rf /usr/local/directadmin/conf/license.key

[root@sucuri ~]# wget -O /usr/local/directadmin/conf/license.key https://raw.githubusercontent.com/LinuxGuard/Directadmin-1.60.4-Nulled/master/license.key

[root@sucuri ~]# chmod 600 /usr/local/directadmin/conf/license.key

[root@sucuri ~]# chown diradmin:diradmin /usr/local/directadmin/conf/license.key

[root@sucuri ~]# ifconfig eth0:92 37.97.247.189 netmask 255.255.255.0 up

[root@sucuri ~]# echo 'DEVICE=eth0:92' >> /etc/sysconfig/network-scripts/ifcfg-eth0:92

[root@sucuri ~]# echo 'IPADDR=37.97.247.189' >> /etc/sysconfig/network-scripts/ifcfg-eth0:92

[root@sucuri ~]# echo 'NETMASK=255.255.255.0' >> /etc/sysconfig/network-scripts/ifcfg-eth0:92

[root@sucuri ~]# systemctl restart network

[root@sucuri ~]# /usr/bin/perl -pi -e 's/^ethernet_dev=.*/ethernet_dev=eth0:92/' /usr/local/directadmin/conf/directadmin.conf

[root@sucuri ~]# systemctl start directadmin

Done:)
