# Opsplash termux
A command line tool unpack/repack oppo/realme/oneplus splash image in termux (android)
## Original https://github.com/affggh/opsplash
## Opsplash
### Issue the permisions
```
termux-setup-storage
``` 
### Install git 
```
pkg update
```
```
pkg install git
```
```
cd /storage/emulated/0
```
### Clone
```
git clone https://github.com/m3myne/opsplash_termux.git
```
```./opsplash unpack -i splash.img -o pic
cd opsplash_termux
```
## Get a splash
### need su
```
su
```
```
dd if=/dev/block/bootdevice/by-name/splash_a of=/storage/emulated/0/opsplash_termux/splash.img
```
## Command Opsplash
### Unpack
```
./opsplash unpack -i splash.img -o pic
```
### Pack
```
./opsplash repack -i splash.img -o new-splash.img
```
### Read info image
```
./opsplash readinfo -i splash.img
```
