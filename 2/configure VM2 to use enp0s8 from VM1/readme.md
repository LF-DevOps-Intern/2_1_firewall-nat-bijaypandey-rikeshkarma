# Configure VM2 to use enp0s8 from VM1

We use the following command in order to configure Ubuntu(VM2) to use enp0s8 from VM1(CentOS):                
`route add default gw 192.168.99.101`              

Lastly use `route` command to observe the IP routing table.       
