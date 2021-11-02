# Solution
To **block certain IP using firewalld** following command was used:            
`firewall-cmd --permanent --add-rich-rule="rule family='ipv4' source address='180.76.15.154' reject"`                    
_'180.76.15.154'_ is taken as a sample and this is a Chinese IP address.                 
        
We have to reload firewalld after adding a permanent rule using the command:                          
`firewall-cmd --reload`                      
