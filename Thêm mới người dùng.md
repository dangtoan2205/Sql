Thêm người dùng mới cho Sql
------------------
```
sudo mysql
```

```
CREATE USER 'snipeit'@'localhost' IDENTIFIED BY 'Adminlocal123a@';
```

```
GRANT ALL PRIVILEGES ON snipeit_db.* TO 'snipeit'@'localhost';
```

```
FLUSH PRIVILEGES;
```

```
CREATE DATABASE snipeit_db;
```

```
exit;
```
