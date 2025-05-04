# 1. Bisa ssh kedalam server dengan contoh command : 
`ssh vm-dumbways`
* masuk ke direktori windows dengan format berikut C:\Users\sakso dan buat file config

![gambar](./images/Screenshot_1.png)

* edit dengan notepad file config dengan settingan seperti ini
```bash
Host vm-dumbways
    HostName 192.168.100.200
    User bay
    Port 22
    IdentityFile ~/.ssh/kunci
```

![gambar](./images/Screenshot_2.png)

* login di terminal dengan perintah vm-dumbways
```bash
ssh vm-dumbways
```

![gambar](./images/Screenshot_3.png)



# 2. Rubah port SSH menjadi 6969
* masuk ke config sshd_config dengan nano

``` bash
sudo nano /etc/ssh/sshd_config
```
![gambar](./images/Screenshot_4.png)

* ganti port 22 menjadi 6969 dan hilangkan simbol hash atau #
* 
![gambar](./images/Screenshot_5.png)

* ganti juga port yang ada di dalam direktori windows
* 
![gambar](./images/Screenshot_6.png)

* setelah itu update systemctl di terminal
  
``` bash
sudo systemctl restart ssh
```

![gambar](./images/Screenshot_7.png)


* exit dan login kembali
  
``` bash
exit
```

``` bash
ssh vm-dumbways
```

![gambar](./images/Screenshot_8.png)

* check koneksi menggunakan lsof
  
``` bash
sudo lsof -i :6969
```

![gambar](./images/Screenshot_9.png)

# 3. SSH hanya bisa diakses 1 device (jika login dari device lain akan bentrok)
* login ke server

* masuk ke direktori dan edit konfigurasi
``` bash
sudo nano /etc/security/limits.conf
```
``` bash
bay maxlogins 1
```

![image](https://github.com/user-attachments/assets/456611c6-2b55-4543-b769-e3b52a838e2c)

* restart ssh dan coba login lagi
``` bash
sudo systemctl restart ssh
```

![image](https://github.com/user-attachments/assets/823cd663-bc56-43f5-ae62-ef64576bd8b7)


