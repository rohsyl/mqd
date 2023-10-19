# MySQL Quick Dump

Dump and restore database quickly with a single command.

## Config

Set a `config` file with database credentials in your current directory

```ini
[database]
host=localhost
port=3306
database=foo
user=bar
password=

[options]
output-dir=
mysql-bin=D:\xampp\mysql\bin\mysql.exe
mysql-dump-bin=D:\xampp\mysql\bin\mysqldump.exe
skip-tables=
snapshot-sub-process-max=15
restore-sub-process-max=1
```

## Take a snapshot
```
mqd snapshot NAME
```

## Restore a snapshot
```
mqd restore NAME
```

## See availables snapshot
```
mqd list
```

## Delete a snapshot
```
mqd delete NAME
```