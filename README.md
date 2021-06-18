# 26thmay_B1_DEVOPS

## BlOCK a specific IP address for ssh
'''
ubuntu@ip-172-31-21-117:~$ sudo iptables -I INPUT -s 172.31.21.117 -p tcp --dport ssh -j REJECT
'''
