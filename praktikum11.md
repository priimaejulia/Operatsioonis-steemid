# Praktikum 11

# ülesanne 11 - 1:

Masin	Liides	IP / prefiks	netmask	network	broadcast
ruuter1	eth0	DHCP (NAT-võrgust)	–	–	–
ruuter1	eth1	192.168.21.1/24	255.255.255.0	192.168.21.0	192.168.21.255
ruuter2	eth0	192.168.21.2/24	255.255.255.0	192.168.21.0	192.168.21.255
ruuter2	eth1	192.168.22.65/26	255.255.255.192	192.168.22.64	192.168.22.127
klient	eth0	192.168.22.66/26	255.255.255.192	192.168.22.64	192.168.22.127

# ülesanne 11 - 2: 

Ruuter 1: 



<img width="356" height="413" alt="pingruuter1" src="https://github.com/user-attachments/assets/13f481fb-d9db-4c7d-a338-27a530fdde2b" />










Ruuter 2:



<img width="320" height="307" alt="pingruuter2" src="https://github.com/user-attachments/assets/40e7f8a1-e9af-48b1-9a59-3debaac822b2" />









Vastus küsimusele: ruuter 2 teab ainult kahte võrku, millega ta on otse ühendatud. Aadress 8.8.8.8 ei kuulu kumbagi neist ja ruuter2-l pole default route'i, mis ütleks kuhu tundmatud paketid saata. Seepärast ei tea ruuter2, kuhu paketti saata, ja annab vea " Network is unreachable"


# ülesanne 11 - 3:

# ülesanne 11 - 4: 
