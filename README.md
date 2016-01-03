# sopcast-script

### Description
Simple script for opening [SopCast](http://www.sopcast.org/) translations in [VLC](http://www.videolan.org/vlc/).

### Installation
You need Sopcast (sp-sc) installed:
```sh
$ wget https://sopcast-player.googlecode.com/files/sp-auth-3.2.6.tar.gz
$ tar xfvz sp-auth-3.2.6.tar.gz
$ sudo cp sp-auth/sp-sc-auth /usr/bin/sp-sc
```

Then try to start sp-sc:
```sh
$ sp-sc
```

If it shows something like that
```sh
$ sp-sc
sp-sc: error while loading shared libraries: libstdc++.so.5: cannot open shared object file: No such file or directory
```
then just install libstdc++.so.5:
```sh
$ wget http://www.sopcast.com/download/libstdcpp5.tgz
$ tar xfvz libstdcpp5.tgz
$ sudo cp -a ./usr/lib/libstdc++.so.5* /usr/lib/
```

And then you can just copy this script to /usr/bin:
```sh
$ git clone https://github.com/supporteam/sopcast-script.git
$ sudo cp sopcast-script/sopcast /usr/bin
$ sudo chmod +x /usr/bin/sopcast
```
Also, you need to have VLC installed. For Debian/Ubuntu/Mint:
```sh
apt-get install vlc
```

It's done!

### Usage
```sh
sopcast sop://broker.sopcast.com:3912/6001
```

That's it!

### Contacts
In case of any questions please contact me on Elance (https://www.elance.com/s/supporteam/), on Skype (supporteam.ru) or by email (me@supporteam.ru).