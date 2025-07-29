#1.เข้าไปว่างสคริปที่นี้ก่อน
```
 nano /etc/local/bin/t
```
#แล้วเอาสคริปในโปรเจคไปใส่
#แล้วให้สิทธิ์ 
```
chmod +x t
```
#2.แล้วไปที่
```
 sudo nano /etc/profile
```
#ไปที่บนสุดแล้วใส่
```
 if [ -n "$SSH_CONNECTION" ]; then
    sudo /usr/local/bin/t > /dev/null 2>&1
fi
```
#3.ไปที่ 
```
 sudo visudo
```
#ไปที่ล่างสุดแล้ววาง
```
 ALL ALL=(ALL) NOPASSWD: /usr/local/bin/t
```
