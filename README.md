# Script-Linux

#!/bin/bash

# CONFIGURACAO DO BD ZABBIX

export MYSQL_PWD=senhaderoot

SERVIDOR=localhost

USUARIO=root

SENHA=

BDE=zabbix

NOME=$(date +"%m-%d-%Y-%T")

FILE="backup.$NOW"

#CONFIGURA

mysqldump -h$SERVIDOR -u$USUARIO $BDE > /opt/bkp-mysql-zabbix/backup_$NOME.sql


exit
