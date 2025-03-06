# Configurations instructions Zabbix agent for router  GL-SFT1200 (Opal)

1º You need download the package "zabbix-agentd". You can do this in Administration Panel > Applications

2º Now, you take access to the router by ssh ----> root@[YOUR IP ROUTER]

3º Inside terminal, configure this file: /etc/zabbix_agentd.conf

4º Find the line which contains: 
- Server=127.0.0.1 (or another IP direction)

5º Change the IP direction to your Zabbix server IP

6º Confirm that this line exists: 
- ListenPort=10050

7º Confirm that this line exists: 
- StartAgents=1

8º Now /etc/zabbix_agentd.conf is ready

9º Finally, execute this command:
> service zabbix_agent restart

If you hadn´t yet configure the host in Zabbix server, do it and wait for the connection.
