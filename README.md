## Port Forwarding
![Alt text](<Port Forwarding.png>)
<br>

-> with NAT you have no easy way of ensuring that outside host can connect to internal web servers or email servers on the correct port such as 80 and 110 <br>
-> Now add port forwarding of NAT configurations on the router<br>
-> We want incoming connections on port 80 for IP 10.0.0.2 to be forwarded to source IP of 172.16.1.2


#### Main Configurations
->Configure terminal <br>
-> ip not inside source static tcp 172.16.1.2 80 10.0.0.2 80<br>
-> interface gigabitEthernet 0/0<br>
-> ip nat inside<br>
-> exit<br>

-> interface gigabitEthernet 0/0<br>
-> ip nat inside
-> exit<br>