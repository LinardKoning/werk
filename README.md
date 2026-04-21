# DNS cheatsheet 
## SPF 
Waarde: 
```
v=spf1 a mx include:_spf.yourfilter.nl -all
```
Waarde: 
```
v=spf1 a mx ip4:<ipv4 adres> a:spf.spamexperts.axc.nl -all
```

## DMARC 

Naam: 
```
_dmarc
```
Waarde: 
```
v=DMARC1; p=quarantine; rua=<email voor bouncemail>;
```

## DKIM 
Naam:
```
_domainkey
``` 
Waarde:
```
o=-
``` 

Naam:
```
default._domainkey
```
Waarde: 
```
v=DKIM1; g=*; k=rsa; p=<private key string>
```
