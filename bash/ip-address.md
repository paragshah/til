# IP Address

Get the IP address

Run this in terminal under any folder you want to serve:
```
ifconfig | grep netmask
```

Better yet, create an alias in your bash profile:
```
alias ip='ifconfig | grep netmask'
```

Then using terminal, enter `ip` to output the IP address of your machine. The output will look like:
```
  inet 127.0.0.1 netmask 0xff000000
  inet 192.168.1.9 netmask 0xffffff00 broadcast 192.168.1.255
```
