# Wiresharkguide
Source: https://github.com/ismailtasdelen/wireshark-cheatsheet.git

+ ```http & ip.src == 192.168.0.1```

+ Management Frame: The frame for the connection between the network device and the client.

+ Control Frame: Controls the integrity of data traffic between the network device and the client.

+ Data Frame: The frame on which the original data is transferred.

Only to show the outgoing packets from the management frame.
 
```
wlan.fc.type==0
```

To show incoming, outgoing packets through control frame.

```
wlan.fc.type==1
```

To show packets transferred over the data frame.

```
wlan.fc.type==2
```

Association lists the requests.

```
wlan.fc.type_subtype==0
```

Association lists the answers.

```
wlan.fc.type_subtype==1
```

Probe lists requests.

```
wlan.fc.type_subtype==4
```

Lists the probe responses.

```
wlan.fc.type_subtype==5
```

Lists Beacon signals / waves.

```
wlan.fc.type_subtype==8
```

Lists the Authentication requests.

```
wlan.fc.type_subtype==11
```

Lists deauthentication requests.

```
wlan.fc.type_subtype==12
```

TCP lists the outgoing packets to the xx port.

```
tcp.port == xx
```

TCP lists packages with the Source xx port.

```
tcp.srcport == xx
```

TCP lists packages with a destination xx port.

```
tcp.dstport == xx
```

UDP lists the outgoing packets to the xx port.

```
udp.port == xx
```

UDP lists packets with a destination xx port.

```
udp.srcport == xx
```

UDP lists packages that have the Source xx port.

```
udp.dstport == xx
```

Lists the HTTP Get requests.

```
http.request
```

Lists packages for the source or destination mac address.

```
wlan.addr == MAC-Address
```

The source lists packages that have a mac address.

```
wlan.sa == MAC-Address
```

Lists packages that have a target mac address.

```
wlan.da == MAC-Address
