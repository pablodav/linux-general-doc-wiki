Init system
===========

* change init:

    `sudo /sbin/telinit 5`


Init process reads /etc/inittab first.

chkconfig is the correct tool to manage init levels, enabling service, etc in RHEL.

### Check service

`chkconfig *service_name*.`

sudo service @--status-all@ to see status of all services.

For Debian/Redhat you need

sudo apt-get install sysvinit-utils chkconfig (on ubuntu you need update-rc.d)

Upstart events are found in /etc/event.d

Ttys started are now configured on /etc/init/start-ttys.conf

initctl also control services and list status.

*systemd*

Status of everything that systemd controls

systemctl 


all available services:

systemctl list-units -t services --all

only active services 

systemctl list-units -t services

ls /lib/systemd/system/*.service to list services possibles. 



