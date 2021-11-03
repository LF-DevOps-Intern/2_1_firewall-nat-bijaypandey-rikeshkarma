# Share connection between VM1 and VM2

`modprobe iptable_nat`           
`echo 1 > /proc/sys/net/ipv4/ip_forward`        
`iptables -t nat -A POSTROUTING -o enp0s3 -j MASQUERADE`         
`iptables -A FORWARD -i enp0s8 -j ACCEPT`        

Above commands are used to share the connection between **VM1(CentOS)** and **VM2(Ubuntu)**.
