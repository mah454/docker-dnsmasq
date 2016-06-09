Docker DNSMasq Service

This service detect all running docker containers and setup dnsmasq service for resolve container's name .

Setup :
1) Install dnsmasq service 
2) Edit /etc/dnsmasq.conf and add this line end of file : 
	addn-hosts=/etc/hosts.docker
3) Copy docker-dnsmasq to /usr/local/sbin 
4) Copy docker-dnsmasq.service to /lib/systemd/system/ 
5) execute this commands : 
	A) systemctl enable docker-dnsmasq.service 
	B) systemctl start dnsmasq 
	C) systemctl start docker-dnsmasq 


Note : 
	/etc/resole.conf muse set to :
		nameserver 127.0.0.1
