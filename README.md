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
# Levon 'noptrix signature 
**[Option](https://github.com/BlackArch/blackarch/issues/4034)**

```bash
sudo echo F9A6E68A711354D84A9B91637533BAFE69A25079:4: >> /usr/share/pacman/keyring/blackarch-trusted
```

```bash
sudo pacman -Syu
```
