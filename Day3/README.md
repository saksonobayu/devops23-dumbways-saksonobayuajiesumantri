# Task Manage Server w/ Terminal
**1. Akses Server menggunakan terminal**
* lakukan instalasi ssh di ubuntu virtualbox
```bash
sudo apt install openssh-server
```
![Screenshot_1](https://github.com/user-attachments/assets/1a697596-8cb7-47ef-93cd-321aae23a780)

* mengecek apakah ssh sudah running atau belum
```bash
sudo systemctl status ssh
```
![Screenshot_2](https://github.com/user-attachments/assets/883ce5ce-46d8-4ec1-bc17-db656c312b25)

* menampilkan semua ip address dengan perintah ip a dan gunakan ip yang inet enp0s3
```bash
ip a
```
![Screenshot_3](https://github.com/user-attachments/assets/47a42681-ceb0-4b55-ac31-d08f763b33b4)


* run terminal windows
  
![image](https://github.com/user-attachments/assets/687f20f7-d46f-4d00-997d-0570cae82dc9)


* melakukan koneksi ssh dari terminal ke server dengan ip sebelumnya
```bash
ssh bay@192.168.100.200
```
![image](https://github.com/user-attachments/assets/084bdccf-203d-4a20-a4fc-72cb55d53da6)


**2. Konfigurasi ssh kalian agar bisa di akses *hanya menggunakan publickey* (password dimatikan)**
* di terminal windows gunakan perintah untuk membuat password dan buat file disini saya buat namanya kunci 
```bash
ssh-keygen
```
![Screenshot_6](https://github.com/user-attachments/assets/cae4e5fc-01b3-4b63-9d1b-f0a87b69b745)


* password akan generate ke dalam direktori file explorer
> C:\Users\sakso\.ssh

![image](https://github.com/user-attachments/assets/ce6031f4-acc4-4c54-9406-44eb368f2aeb)


* buka file kunci.pub dan copy ssh publik tersebut
![image](https://github.com/user-attachments/assets/40bcffa4-c95e-4c85-aa2a-906d39a18875)


* masuk ke server dari terminal lalu gunakan perintah 
```bash
cd .ssh
```
![Screenshot_7](https://github.com/user-attachments/assets/e84255fe-05c1-4148-ad46-580c48704f90)


* masuk ke dalam file authorize_keys dengan nano dan tempel ssh publik yang sudah dicopy kemudian di simpan
```bash
nano authorize_keys
```
![Screenshot_8](https://github.com/user-attachments/assets/98bc21e8-53e7-450f-a6c0-959fac2e1aea)
![image](https://github.com/user-attachments/assets/b564254d-e331-4f37-a819-04da56f19386)


* terminal windows lalu gunakan perintah untuk akses server tanpa perlu login password 
```bash
ssh -i .ssh/kunci bay@192.168.100.200
```
![Screenshot_9](https://github.com/user-attachments/assets/c541de4c-a075-4cdd-b755-679828f4ff9b)


**3. Buat step by step penggunaan text manipulation! (grep, sed, cat, echo)**
* menggunakan perintah cat untuk replace text di dalam file tertentu
```bash
cat berkassatu
cat > berkassatu
hello
```
![image](https://github.com/user-attachments/assets/83797527-a26b-4d19-9169-9b14d2f5be3b)


* menggunakan perintah cat untuk menggabungkan text
```bash
cat berkassatu
cat berkasdua
cat berkastiga
```
```bash
cat berkassatu berkasdua berkastiga > berkasempat
```
![image](https://github.com/user-attachments/assets/9d169bc3-adbc-410d-8b4e-3d3d6e3ef31e)

* menggunakan perintah echo untuk print text ke terminal
```bash
echo "oh hi"
```
![image](https://github.com/user-attachments/assets/59997856-0291-468d-90e1-6f81abf5dda3)


* menggunakan perintah echo untuk replace text di dalam file
```bash
cat berkasdua
echo "oh hi" > berkasdua
```
![image](https://github.com/user-attachments/assets/df380e41-4cee-45f5-a3c1-ec2ddfaeb94d)


* menggunakan perintah echo untuk menambah text di dalam file
```bash
cat berkasdua
echo "oh hi" >> berkasdua
```
![image](https://github.com/user-attachments/assets/a140cea0-f9f0-4d55-8788-3dedcd5436f4)

* menggunakan perintah echo untuk membuat file baru dengan text didalamnya
```bash
cat berkaslima
echo "hm" > berkaslima
ls
cat berkaslima
```
![image](https://github.com/user-attachments/assets/53f835d1-c5f7-495a-9d45-bfa7b09ad471)

* menggunakan perintah grep untuk mencari pola text di dalam text atau input
```bash
grep hi berkasdua
```
![image](https://github.com/user-attachments/assets/fa058e46-3818-4bb5-9eee-91c1b902ad6d)

* menggunakan perintah grep untuk mencari pola text case sensitive
```bash
echo -e "hello\nHELLO\nHello\nhElLo" > berkastujuh.txt
```
```bash
cat berkastujuh.txt
```
```bash
grep "hello" berkastujuh.txt
```
```bash
grep -i "hello" berkastujuh.txt
```
manfaat dari perintah insensitive atau -i adalah dapat mencari text error dimana developer tidak memperhatikan uppercase dan lowercase 
![image](https://github.com/user-attachments/assets/9954c25f-d07b-4ef4-974e-8e0d7031491d)

* menggunakan perintah grep untuk menghitung kata yang sama
```bash
grep -c hi berkasdua
```
![image](https://github.com/user-attachments/assets/00362939-4ec9-4863-bdfd-265deaf3edcd)

```bash
grep -c hi *
```
![image](https://github.com/user-attachments/assets/cc3ff9ae-5bc7-4ef9-b737-78da7f13bd2f)


* menggunakan perintah grep untuk menampilkan baris angka
```bash
grep -n hi berkasdua
```
![image](https://github.com/user-attachments/assets/162cb6d3-5502-46fe-bdf1-34f7f6653e80)


**4. Nyalakan ufw dengan memberikan akses untuk port 22, 80, 443, 3000, 5000 dan 6969**
* menggunakan perintah ufw allow untuk menginzinkan akses uncomplicated firewall
```bash
sudo ufw allow 22
```
```bash
sudo ufw allow 80
```
```bash
sudo ufw allow 443
```
```bash
sudo ufw allow 3000
```
```bash
sudo ufw allow 5000
```
```bash
sudo ufw allow 6969
```
```bash
sudo ufw status
```
![image](https://github.com/user-attachments/assets/eff35383-910b-4a8f-a3cf-9bef0be7e16f)

