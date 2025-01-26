# Zabbix Postfix template

## Description

Template to monitor Postfix installations. For the template to count spammy mails it is recommended to use amavis/spamassassin withing yout postfix setup.


## Installation notes

1. Set right path to your postfix mail.log ({$LOGPATH}) file in template Macros section
2. Set right postfix service name ({$SYSTEMD.NAME.SERVICE.MATCHES}) in template Macros section

## Items collected

|Name|Description|Type|
|----|-----------|----|
|Connections|Number of socket connections to postfix server|Numeric(unsigned)|
|Received mail|Number of mails received|Numeric(unsigned)|
|Received spam|Number of mails received classified as spam (spamassassin required)|Numeric(unsigned)|
|Rejected mail|Number of mails rejected by postfix|Numeric(unsigned)|
|Sent mail|Number of mails sent by postfix|Numeric(unsigned)|
|Active state|State value that reflects whether the service is currently active or not|Numeric(unsigned)|
|Active time|Number of seconds since service entered the active state|Numeric(float)|
|Load state|State value that reflects whether the configuration file of the service has been loaded|Numeric(unsigned)|
|Unit file state|Encodes the install state of the service file of FragmentPath|Numeric(unsigned)|
