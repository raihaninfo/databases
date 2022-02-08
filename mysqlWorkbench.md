## MySql

> sudo apt update

> sudo apt install mysql-server

> sudo mysql_secure_installation utility

```
sudo ufw enable
sudo ufw allow mysql
```

> CREATE USER 'username'@'host' IDENTIFIED WITH authentication_plugin BY 'password';

```

CREATE USER 'raihan'@'localhost' IDENTIFIED BY 'password';
```

> GRANT PRIVILEGE ON database.table TO 'username'@'host';

```
GRANT CREATE, ALTER, DROP, INSERT, UPDATE, DELETE, SELECT, REFERENCES, RELOAD on *.* TO 'raihan'@'localhost' WITH GRANT OPTION;
```

## Mysql Workbench

[Download](https://dev.mysql.com/downloads/file/?id=509020)

```
cd Downloads
```

```
sudo apt install ./mysql-apt-config_0.8.16-1_all.deb
```

```
sudo apt install mysql-workbench-community
```
