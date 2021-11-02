# Solution
To **allow http, https and ssh** connection using firewall, we use the following commands respectively:                     
`firewall-cmd --zone=public --add-service=http`                 
`firewall-cmd --zone=public --add-service=https`                       
`firewall-cmd --zone=public --add-service=ssh`                       
                       
The above rules will be removed after system reboot. We need to use the --permanent option to save the rules permanently as listed below:                   
`firewall-cmd --permanent --zone=public --add-service=http`                 
`firewall-cmd --permanent --zone=public --add-service=https`       
`firewall-cmd --permanent --zone=public --add-service=ssh`              
