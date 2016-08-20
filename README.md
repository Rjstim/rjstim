# rjstim

Удаление PostgreSQL из под Ubuntu

Выполняем последовательность команд. Последовательность избыточна. В зависимости от того, как эксплуатировалась база некоторые команды могут сообщить, что они ничего полезного не сделали.

sudo apt-get --purge remove pgadmin3
sudo apt-get --purge remove postgresql\*

sudo rm -r /etc/postgresql/
sudo rm -r /etc/postgresql-common/
sudo rm -r /var/lib/postgresql/
sudo userdel -r postgres
sudo groupdel postgres


