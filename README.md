# pdns-recursor

Docker image with local dns recursor.
Based on debian:stable and pdns-recursor.

It exposes 53 and 53/udp ports.

# How to run it?

```
$ sudo docker run --rm --name pdns-recursor -p 127.0.0.1:53:53 -p 127.0.0.1:53:53/udp antage/pdns-recursor -d
$ echo "nameserver 127.0.0.1" > sudo tee /etc/resolv.conf
```
