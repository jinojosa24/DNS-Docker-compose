# DNS-Docker-compose
## 1 Configura un contenedor coa imaxe oficial de bind9 usando docker-compose.


## 2 Usa os volumes como se explica no setup da imaxe



## 3 Unha comprobado que o contenedor funciona, sube a GitHub o ficheiro nun repo.


## 4 Pega na resposta o enlace ó repo.
jose@jose-VirtualBox:~$ dig @172.20.0.2

; <<>> DiG 9.18.28-0ubuntu0.22.04.1-Ubuntu <<>> @172.20.0.2
; (1 server found)
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 8365
;; flags: qr rd ra ad; QUERY: 1, ANSWER: 13, AUTHORITY: 0, ADDITIONAL: 27

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 1232
; COOKIE: 881cb6c081f63dcc01000000672131b76478ca804455367e (good)
;; QUESTION SECTION:
;.				IN	NS

;; ANSWER SECTION:
.			518399	IN	NS	g.root-servers.net.
.			518399	IN	NS	b.root-servers.net.
.			518399	IN	NS	k.root-servers.net.
.			518399	IN	NS	f.root-servers.net.
.			518399	IN	NS	c.root-servers.net.
.			518399	IN	NS	j.root-servers.net.
.			518399	IN	NS	h.root-servers.net.
.			518399	IN	NS	a.root-servers.net.
.			518399	IN	NS	e.root-servers.net.
.			518399	IN	NS	d.root-servers.net.
.			518399	IN	NS	i.root-servers.net.
.			518399	IN	NS	l.root-servers.net.
.			518399	IN	NS	m.root-servers.net.

;; ADDITIONAL SECTION:
a.root-servers.net.	518399	IN	A	198.41.0.4
b.root-servers.net.	518399	IN	A	170.247.170.2
c.root-servers.net.	518399	IN	A	192.33.4.12
d.root-servers.net.	518399	IN	A	199.7.91.13
e.root-servers.net.	518399	IN	A	192.203.230.10
f.root-servers.net.	518399	IN	A	192.5.5.241
g.root-servers.net.	518399	IN	A	192.112.36.4
h.root-servers.net.	518399	IN	A	198.97.190.53
i.root-servers.net.	518399	IN	A	192.36.148.17
j.root-servers.net.	518399	IN	A	192.58.128.30
k.root-servers.net.	518399	IN	A	193.0.14.129
l.root-servers.net.	518399	IN	A	199.7.83.42
m.root-servers.net.	518399	IN	A	202.12.27.33
a.root-servers.net.	518399	IN	AAAA	2001:503:ba3e::2:30
b.root-servers.net.	518399	IN	AAAA	2801:1b8:10::b
c.root-servers.net.	518399	IN	AAAA	2001:500:2::c
d.root-servers.net.	518399	IN	AAAA	2001:500:2d::d
e.root-servers.net.	518399	IN	AAAA	2001:500:a8::e
f.root-servers.net.	518399	IN	AAAA	2001:500:2f::f
g.root-servers.net.	518399	IN	AAAA	2001:500:12::d0d
h.root-servers.net.	518399	IN	AAAA	2001:500:1::53
i.root-servers.net.	518399	IN	AAAA	2001:7fe::53
j.root-servers.net.	518399	IN	AAAA	2001:503:c27::2:30
k.root-servers.net.	518399	IN	AAAA	2001:7fd::1
l.root-servers.net.	518399	IN	AAAA	2001:500:9f::42
m.root-servers.net.	518399	IN	AAAA	2001:dc3::35

;; Query time: 0 msec
;; SERVER: 172.20.0.2#53(172.20.0.2) (UDP)
;; WHEN: Tue Oct 29 20:04:23 CET 2024
;; MSG SIZE  rcvd: 851

jose@jose-VirtualBox:~$ 
