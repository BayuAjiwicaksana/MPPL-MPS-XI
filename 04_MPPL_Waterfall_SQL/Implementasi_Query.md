# Implementasi Query SQL

## Membuat Database
Database yang akan saya buat memiliki nama **mppl_waterfall_sql**.
Query :
```
mysql> CREATE DATABASE mppl_waterfall_sql;
```

## Membuat User Baru
User baru yang akan saya buat memiliki *username* = **bayu**, dan *password* = **qwerty**.
Query :
```
mysql> CREATE USER ‘bayu’@’localhost’ IDENTIFIED BY ‘qwerty’;
```

## Memberikan Hak Akses untuk Database ke User
User **bayu** akan diberikan hak akses penuh untuk database **mppl_waterfall_sql**.
Query :
```
mysql> GRANT ALL PRIVILEGES ON mppl_waterfall_sql.* TO ‘bayu’@’localhost’;
```

## Masuk menggunakan User Baru dan menggunakan database
Query :
```
mysql -u bayu -p
mysql> USE mppl_waterfall_sql;
Database changed
```