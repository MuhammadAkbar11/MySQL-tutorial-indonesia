## Tabel

### Storage Egines

MySQL memilik berbagai cara melakukan pengolahan data, hal ini disebut Storage Engines, saat ini yang biasa dan populer digunakan adalah InnoDB

Untuk melihat Storage Engines apa saja yang terdapat di MYSQL, Bisa menggunakan perintah

```bash
mysql> SHOW ENGINES;
```

<br>

### Membuat Tabel

Perintah membuat sebuah Tabel

```bash
# Tekan Shift+Enter untuk membuat baris baru pada terminal
mysql> CREATE TABLE table_name
    -> (
    -> column1 INT,
    -> column2 VARCHAR(128),
    -> column3 INT,
    -> column4 INT
    -> ) ENGINE = InnoDB;
```

<br>
