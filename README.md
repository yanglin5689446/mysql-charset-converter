## mysql-charset-converter
Convert all tables (including database itself) to specific charset (and collation)

## Install
```
curl -GO "https://raw.githubusercontent.com/yanglin5689446/mysql-charset-converter/master/mysql-charset-converter"
```
...then move downloaded script to any executable path you like, or use it one-shot

### Usage
```
mysql-charset-converter [-H host] [-u user] [-p password] [-c charset] [-C collation] database
```
#### args
- host: optional, default=`localhost`
- user: optional, default=`root`
- password: optional, default=``
- charset: required
- collation: optional

#### TL;DR
Pretty much everyone just wants to convert utf8 to utf8mb4 I guess
```
mysql-charset-converter -h <host> -u <user> -p <password> -c utf8mb4 -C utf8mb4_general_ci <database>
```
