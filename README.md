# Python2.7-MySQLdb-my_config.h
_mysql.c:44:10: fatal error: my_config.h: No such file or directory

## Introduction
If running the pip script shows the following error message:
```bash=
$ pip install MySQL-python
...
_mysql.c:44:10: fatal error: my_config.h: No such file or directory
...
```

Copy the my_config.h file to /usr/include/mysql/
```bash=
$ sudo wget https://raw.githubusercontent.com/SyXuan/Python2.7-MySQLdb-my_config.h/main/my_config.h -P /usr/include/mysql/
```

## Reference
https://stackoverflow.com/questions/62087499/failing-to-install-mysql-python  
Forked from https://github.com/paulfitz/mysql-connector-c  