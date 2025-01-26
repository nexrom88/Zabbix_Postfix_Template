# Zabbix Postfix template

## Description

Template to monitor Postfix installations. For the template to count spammy mails it is recommended to use amavis/spamassassin withing yout postfix setup.


##Installation notes

1. Set right path to your postfix mail.log ({$LOGPATH}) file in template Macros section
2. Set right postfix service name ({$SYSTEMD.NAME.SERVICE.MATCHES}) in template Macros section

##Collected items
## Items collected

|Name|Description|Type|
|----|-----------|----|
|Connections|Number of socket connections to postfix server|Numeric(unsigned)|
