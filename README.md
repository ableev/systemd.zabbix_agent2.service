# systemd.zabbix_agent2.service

cp /tmp/zabbix_agent2.service /usr/lib/systemd/system/zabbix_agent2.service

ln -nsf /usr/lib/systemd/system/zabbix_agent2.service /etc/systemd/system/multi-user.target.wants/zabbix_agent2.service

systemctl daemon-reload

systemctl stop zabbix-agent

systemctl disable zabbix-agent

systemctl start zabbix_agent2
