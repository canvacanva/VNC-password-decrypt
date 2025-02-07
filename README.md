# VNC-password-decrypt

From linux machine:
```
echo -n d7a514d8c556aade | xxd -r -p | openssl enc -des-cbc --nopad --nosalt -K e84ad660c4721ae0 -iv 0000000000000000 -d -provider legacy -provider default | hexdump -Cv
```
where "d7a514d8c556aade" is psw export from vnc profile 
