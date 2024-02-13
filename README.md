# Black-Arch-Solutions
[BlackArch download](https://blackarch.org/)


# Invalid or Corrupted Package (PGP Signature)
**[Option 1:](https://blackarch.org/faq.html)**

```bash
rm -rf /etc/pacman.d/gnupg
```

```bash
pacman-key --init
```

```bash
pacman-key --populate archlinux blackarch
```

```bash
pacman-key --update --keyserver keyserver.ubuntu.com
```
```
sudo pacman -S archlinux-keyring
```
```
sudo pacman -Syu
```
# Levon 'noptrix signature 
**[Option](https://github.com/BlackArch/blackarch/issues/4034)**

```bash
sudo echo F9A6E68A711354D84A9B91637533BAFE69A25079:4: >> /usr/share/pacman/keyring/blackarch-trusted
```

```bash
sudo pacman -Syu
```
# Conflicting files
```
uvicorn: /usr/bin/uvicorn exists in filesystem (owned by python-uvicorn)
```
```
yay -Rns python-uvicorn theharvester
```
```
sudo pacman -Syu
```
# Burp Suite Error
```bash
sudo pacman -S yay
```
```bash
yay -Ss openjdk17
```
```bash
yay -S nombre_del_paquete
```
```bash
pwd: cd /usr/lib/jvm
ls
java-17-j9
```
```bash
sudo archlinux-java set java-17-j9/
java -version
```
