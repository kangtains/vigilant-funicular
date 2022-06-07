# 1Password

Aplikasi 1Password Linux tersedia untuk semua distribusi Linux utama termasuk Ubuntu, Fedora, dan Arch.

Anda dapat menambahkan repo 1Password resmi ke sistem Anda untuk menginstalnya menggunakan manajer paket pilihan Anda, tetapi cara termudah untuk menginstal 1Password di Ubuntu adalah dengan mengunduh paket penginstal di bawah, dan menginstalnya menggunakan aplikasi Perangkat Lunak Ubuntu.

Meskipun tersedia, aplikasi Snap 1Password tidak memiliki integrasi browser web serta metode otentikasi sistem yang mendasarinya. Ini menjadikannya pilihan yang kurang menarik daripada paket instal biasa yang tersedia IMO, tetapi ada jika Anda menginginkannya.

## 1Password for Linux supports

- Automatic Dark Mode selection based on your GTK theme

- Open network locations (FTP, SSH, SMB)
- Integration with GNOME, KDE, and other window managers
- System tray icon
- Open and fill in your default browser
- X11 clipboard integration and clearing
- GNOME Keyring and KDE Wallet support
- Kernel keyring integration
- DBUS API support
- Command line API
- Integration with system lock and idle services

## Installasi

Pertama instal curl dengan menjalankan perintah di bawah ini:

```shell
sudo apt update
```

```shell
sudo apt install curl
```

Next, add 1Password repository key to Ubuntu/Debian

```shell
curl -sS https://downloads.1password.com/linux/keys/1password.asc | sudo gpg --dearmor --output /usr/share/keyrings/1password-archive-keyring.gpg
```

Then create a repository file.

```shell
echo 'deb &#91;arch=amd64 signed-by=/usr/share/keyrings/1password-archive-keyring.gpg] https://downloads.1password.com/linux/debian/amd64 stable main' | sudo tee /etc/apt/sources.list.d/1password.list
```
To verify packages signatures and make sure they’re authentic, add lines below:

```shell
sudo mkdir -p /etc/debsig/policies/AC2D62742012EA22/
```

```shell
curl -sS https://downloads.1password.com/linux/debian/debsig/1password.pol | sudo tee /etc/debsig/policies/AC2D62742012EA22/1password.pol
```

```shell
sudo mkdir -p /usr/share/debsig/keyrings/AC2D62742012EA22
```

```shell
curl -sS https://downloads.1password.com/linux/keys/1password.asc | sudo gpg --dearmor --output /usr/share/debsig/keyrings/AC2D62742012EA22/debsig.gpg
```

Terakhir, jalankan perintah di bawah ini untuk memperbarui dan menginstal 1Password

```shell
sudo apt update & sudo apt install 1password
```

##### Source

- [fossbytes.com](https://fossbytes.com/how-to-install-1password-on-linux/)