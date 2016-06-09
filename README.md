Docker DNSMasq Service<br />

This service detect all running docker containers and setup dnsmasq service for resolve container's name .<br />

**Setup :**<br />

1. Install dnsmasq service<br /> 
2. Edit /etc/dnsmasq.conf and add this line end of file :<br />
```
addn-hosts=/etc/hosts.docker
```
3. Copy docker-dnsmasq to /usr/local/sbin<br /> 
4. Copy docker-dnsmasq.service to /lib/systemd/system/<br /> 
5. execute this commands : <br />
```
systemctl enable docker-dsmasq.service 
systemctl start dnsmasq
systemctl start docker-dnsmasq 
```

**Note :**<br />
	/etc/resole.conf :<br />
```
nameserver 127.0.0.1
```