# Buid môi trường linux cơ bản để dev

```bash
sudo apt install build-essential
sudo apt update && sudo apt full-upgrade -y
```
# Đổi phân vùng ghi wsl2 - mở cmd

```bash
wsl --export <name distro> .....\ubuntu.tar
```
	**example:  wsl --export D:\WSL\ubuntu.tar**
```bash
wsl --unregister <name distro>
```
	**example: wsl --unregister Ubuntu**

**cd ra đường dẫn vừa export**
```bash
wsl --import <new name distro> <path giải nén> <path file nén>
```
	example: wsl --import Ubuntu_z .\ .\ubuntu.tar

**How to use?**

**open: cmd**
```bash
wsl -u <username>
```
	**example: wsl -u yourname**
xong **cd** là ra dc file gốc trên wsl

# Git lưu cache 

``` bash
$ git config --global credential.helper cache
```
# Git xoá cache

```bash
$ git config --global --unset credential.helper
$ git config --system --unset credential.helper
```
