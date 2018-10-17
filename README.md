# AUTO INSTALLER SHADOWSOCKS ON GOOGLE CLOUD PLATFORM

Auto Installer ShadowSocks on Google Cloud Platform

# Requirement System

[SERVER]
- Google Cloud Platform 
- Ubuntu Server OS (16.04 - 18.04) LTS
- IP Static Public
- Open Port 8838 or own port

[CLIENT]
- Min. Windows 7 (x86/x64)
- Browser (Google Chrome/Mozilla Firefox)

# USAGE

[login SSH as root]
```
sudo -i
```
[clone repository]
```
git clone https://github.com/chiho10/auto-shadowsocks-gcp.git
```
[open directory]
```
cd auto-shadowsocks-gcp
```
[change permission]
```
chmod +x autoinstall.sh
```
[run script]
```
./autoinstall.sh
```
[change own server port & password]
```
nano /etc/shadowsocks/shadowsocks.json
```
```
{
    "server":"0.0.0.0",
    "server_port":8838,     #change your own shadowsocks server port
    "password":"123456",    #change your own shadowsocks password
    "timeout":300,
    "method":"aes-256-cfb", #change your own shadowsocks method
    "fast_open": true
}
```
- save with ctrl+O & enter, exit ctrl+x

- reboot your vps

Done.
