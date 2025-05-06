# Load Balancing Nginx
**1. Running node js dari user bay dan ajie**
```bash
cd wayshub-frontend
nvm use 13
npm start
```
![image](https://github.com/user-attachments/assets/e4558331-57ab-4f89-bad3-433a049088e0)

![image](https://github.com/user-attachments/assets/6884cbfe-d37d-4fe4-b5bc-7d363aefafa7)

**2. Masuk ke file bayu.conf**
```bash
sudo nano /etc/nginx/sites-available/bayu.conf
```

![image](https://github.com/user-attachments/assets/03b6ccb3-7df6-4aee-80d0-34ca5cdd4aec)

**3. Update konfigurasinya untuk kedua server sekaligus deklarasi log untuk monitoring**
```bash
log_format upstream_log '$server_name to: $upstream_addr [$request] '
                       'upstream_response_time $upstream_response_time '
                       'msec $msec request_time $request_time';

upstream bayu {
    server 192.168.100.200:3000;
    server 192.168.100.150:3000;
}

server {
    server_name bayu.xyz;


    access_log /var/log/nginx/access.log upstream_log;

    location / {
        proxy_pass http://bayu;
    }
}
```
![image](https://github.com/user-attachments/assets/6b80a38e-4508-46ab-a5ff-05cdd0121b61)

**4. Mengecek code dan restart**

```bash
sudo nginx -t
sudo systemctl reload nginx
```

![Screenshot_22](https://github.com/user-attachments/assets/854c31b8-f986-41c9-874f-8c9bcf03a90c)

![image](https://github.com/user-attachments/assets/25d13c5f-af91-493b-83df-abc1bb758ff2)

**5. Buka log untuk monitoring**
```bash
sudo tail -f /var/log/nginx/access.log
```

**6. Buka browser dan akses bayu.xyz kemudian refresh beberapa kali**

![image](https://github.com/user-attachments/assets/6ea62b1c-cfa8-4aae-96f1-46d8861b1a44)


**7. Buka kembali terminal untuk melihat log**

![Screenshot_23](https://github.com/user-attachments/assets/db8d749f-f153-4f41-84ea-cff40b216781)
