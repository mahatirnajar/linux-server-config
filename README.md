# Konfigurasi Server Linux

Akses server melalui ssh kemudian lakukan update dan upgrade.&#x20;

```
apt-get update && apt-get upgrade
```

Buat hostname baru

```
hostnamectl set-hostname user
```

Selanjutnya kita perlu menambahkan hostname yang baru ke file hosts

```
nan0 /etc/hosts
```

akan tampak tampilan seperti di bawah ini, selanjutnya tambahkan ip address dan hostname yang baru saja kita buat ke file ini.

![](.gitbook/assets/image.png)

Selanjutnya kita perlu membuat user selain root.

```
adduser mahatir
```

Selanjutnya agar user mahatir dapat menggunakan command `sudo` maka kita perlu menambahkan user tersebut ke dalam group sudo.

```
adduser mahatir sudo
```

Logout kemudian ssh kembali ke server menggunakan user baru. Pastikan posisi berada di direktori user didalam home kemudian buat direktori .ssh.&#x20;
