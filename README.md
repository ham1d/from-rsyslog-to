# rsyslog TAG forwarder

## What is this:
This is simple configuration for rsyslog that extract specific tag from log files and send it to any remote server.

## How to use:
Replace this file with original rsyslog config in `/etc/rsyslog.conf` and restart rsyslog service using `systemctl restart rsyslog`

## Optimization
`if $msg contains 'AVR' then @@192.168.74.199:514`
Replace your TAG and remtoe server address in rsyslog.conf file
