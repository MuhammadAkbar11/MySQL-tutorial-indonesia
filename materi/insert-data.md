## Insert Data

untuk memasukan data kedalam tabel, kita bisa menggunakan perintah SQL yang beranama INSERT. Ketika ingin memasukan data kedalam tabel, pastikan tabel sudah dibuat.

```sh
# contoh membuat tabel
mysql> CREATE TABLE products (
    -> id           VARCHAR(10) NOT NULL,
    -> name         VARCHAR(128) NOT NULL,
    -> description  TEXT,
    -> price        INT UNSIGNED NOT NULL,
    -> quantity     INT UNSIGNED NOT NULL DEFAULT 0,
    -> created_at   TIMESTAMP NOT NULL DEFAULT CURRENT_TIMESTAMP
    -> ) ENGINE = InnoDB;
```

### Memasukan single data

```sh
mysql> INSERT INTO table_name(id, name, price, quantity) VALUES ("P0001", "colomn name", 20000, 100);
```

### Memasukan Multiple data

```sh
mysql> INSERT INTO table_name(id, name, price, quantity)
    -> VALUES ("P0001", "colomn name 1", 15000, 100),
    -> ("P0002", "colomn name 2", 17000, 100),
    -> ("P0003", "colomn name 3", 23000, 100);
```

<br><br><br>

[Kembali ke daftar meteri ](./../README.md)
