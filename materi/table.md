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

### Melihat Struktur Tabel

Perintah melihat struktur sebuah tabel

```sh
mysql> DESCRIBE table_name;
#or
mysql> DESC table_name;
```

Perintah melihat struktur tabel dalam sintaks pembuatan tabelnya

```sh
mysql> SHOW CREATE TABLE table_name;
```

<br>

### Mengubah Tabel

#### Perintah-perintah mengubah struktur sebuah tabel

##### Menambahkan kolom baru

```bash

mysql> ALTER TABLE table_name ADD COLUMN new_coloumn TEXT;
```

##### Menghapus kolom

```bash
mysql> ALTER TABLE table_name DROP COLUMN coloum CHAR;
```

##### Menghapus kolom

```bash
mysql> ALTER TABLE table_name ADD COLUMN new_coloumn TEXT;
```

#### Mengubah nama kolom

```sh
mysql> ALTER TABLE table_name RENAME COLUMN old_name to new_name
```

#### Mengubah tipe kolom

```sh
mysql> ALTER TABLE table_name MODIFY coloum2 VARCHAR(128) AFTER column1;
#or
mysql> ALTER TABLE table_name MODIFY coloum2 VARCHAR(128) FIRST;
```
