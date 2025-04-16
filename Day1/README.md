### List Task :

1. Jelaskan istilah DevOps dengan kata kunci : Continuous

2. Buatlah 1 Virtual Machine (bebas ingin menggunakan Multipass, VMware, Virtualbox, etc)

3. Install Nginx WebServer ke dalam Virtual Machine yang telah kalian buat.

---

### TASK 1
>Istilah continuous dalam devops adalah integrasi dan otomatisasi yang berkelanjutan pada semua tahap pengembangan perangkat lunak.

### 1. Continuous Integration
Proses menggabungkan kode dari developer ke repositori utama secara berkelanjutan
**Purpose**
- mengetahui bug lebih dini
- memvalidasi kode selalu siap ke tahap berikutnya

### 2. Continuous Delivery
Proses untuk memastikan kode siap di deploy setiap saat
**Purpose**
- mengurasi resiko rilis
- mempersingkat waktu rilis

### 3. Continuous Deployment
Proses untuk memastikan kode dapat di deploy secara otomatis
**Purpose**
- menghilangkan intervensi manual
- pengiriman fitur lebih cepat

### 4. Continuous Testing
Proses pengujian otomatis sepanjang tahap pengembangan
**Purpose**
- memvalidasi kualitas kode
- meminimalisir bug yang menumpuk

### 5. Continuous Monitoring
Pemantauan performa aplikasi dan infrastruktur secara real time
**Purpose**
- mengetahui masalah lebih dini sebelum berdampak ke pengguna
- memberikan evaluasi untuk maintenance berkelanjutan
---

### TASK 2

# Panduan Instalasi Ubuntu Server di VirtualBox

## Langkah 1: Download Ubuntu Server

Download Ubuntu Server di [https://ubuntu.com/download/server](https://ubuntu.com/download/server)

## Langkah 2: Download VirtualBox

Download VirtualBox di [https://www.virtualbox.org/](https://www.virtualbox.org/)

## Langkah 3: Install VirtualBox

Lakukan installasi VirtualBox.

## Langkah 4: Install Ubuntu Server di VirtualBox

Lakukan installasi Ubuntu Server di VirtualBox.
![Screenshot_1](https://github.com/user-attachments/assets/c12c35c1-4132-4fa3-951f-07d328952962)

## Langkah 5: Pilih Opsi Instalasi

Pilih "Skip Unattended Installation".
![Screenshot_2](https://github.com/user-attachments/assets/379545d2-9983-4c57-9207-594ddc5b38ca)


## Langkah 6: Atur Memori

Set memory sesuai yang direkomendasikan yaitu 2048 MB.
![Screenshot_3](https://github.com/user-attachments/assets/5420380c-8d3b-4380-b0b3-68ad7d5ade62)


## Langkah 7: Atur Hard Disk

Set hard disk sebesar 10 GB lalu pilih finish.
![Screenshot_4](https://github.com/user-attachments/assets/8b175fb4-0436-4092-b7e3-c9e18b230f68)


## Langkah 8: Start Ubuntu Server

Start Ubuntu Server dari dalam virtual box
![Screenshot_5](https://github.com/user-attachments/assets/9557f340-fdf1-404a-ab5d-f538a4bfd6ad)


## Langkah 9: Pilih Instalasi

Pilih try or install Ubuntu Server dan tunggu proses installasi.
![Screenshot_5](https://github.com/user-attachments/assets/20ba060f-92a5-441a-830d-c0590deedc3b)


## Langkah 10: Pilih Bahasa

Masuk ke proses instalasi pilih Bahasa English.
![Screenshot_6](https://github.com/user-attachments/assets/d304c2e7-c3d1-4c41-9de2-c84017e93dba)


## Langkah 11: Lanjutkan Tanpa Update

Pilih continue without updating.
![Screenshot_7](https://github.com/user-attachments/assets/69880673-bdce-4e6d-ac64-c4c7bdfc1a77)

## Langkah 12: Pilih Keyboard

Pilih keyboard us untuk setting keyboard
![Screenshot_8](https://github.com/user-attachments/assets/9aaf70df-be92-42f5-a296-8688c9ee2df5)


## Langkah 13: Pilih Ubuntu Server

Pilih Ubuntu Server yang paling atas.
![Screenshot_9](https://github.com/user-attachments/assets/3d581952-a634-441b-b508-f6ee856cfd3a)


## Langkah 14: Atur Koneksi Manual

Atur koneksi secara manual dengan memilih enp0s3 > edit ipv4.
![Screenshot_10](https://github.com/user-attachments/assets/c8805955-437f-4216-abf2-6fc5b07b53fb)


## Langkah 15: Pilih Metode IP Manual

Pilih ipv4 method manual untuk mengatur koneksi
![Screenshot_11](https://github.com/user-attachments/assets/3b722064-80cb-436f-8297-9d2cc863e942)


## Langkah 16: Masukkan Konfigurasi IP

Masukkan ip config dari desktop Windows lewat cmd dengan prompt "ip config".
![image](https://github.com/user-attachments/assets/446db0d2-8878-4f70-8436-fb859be14d1b)


Pilih sesuai koneksi yang terhubung misal ethernet atau wifi karena di demo ini menggunakan koneksi wifi maka pengisian disesuaikan.
![Screenshot_12](https://github.com/user-attachments/assets/56b86feb-547d-41d9-aaa3-3af6c8ff3734)
![Screenshot_13](https://github.com/user-attachments/assets/eba1de6d-9016-4275-8eb0-988c1c61310e)
![Screenshot_14](https://github.com/user-attachments/assets/0b215ee8-4528-4f0a-b3a9-dfab187a7882)


## Langkah 17: Set DNS

Set DNS ke "8.8.8.8, 8.8.4.4" untuk menghubungkan ke koneksi Google kemudian save.
![Screenshot_14](https://github.com/user-attachments/assets/c67af95c-8db5-4302-8bcd-eb13527aa921)


## Langkah 18: Selesaikan Konfigurasi Jaringan

Setelah itu pilih done untuk melanjutkan proses installasi.
![Screenshot_15](https://github.com/user-attachments/assets/57e05669-e8d8-4c6c-9ff2-6b62f255c4b4)


## Langkah 19: Lewati Konfigurasi Proxy

Untuk tahap proxy configuration dapat di skip.
![Screenshot_17](https://github.com/user-attachments/assets/99ae2f0d-bb7a-42e2-a76a-14bcfef2f8e7)


## Langkah 20: Lewati Konfigurasi Mirror

Untuk tahap Ubuntu archive mirror configuration dapat di skip.
![Screenshot_18](https://github.com/user-attachments/assets/5b83982b-fc87-46e3-874a-15ded7757b84)


## Langkah 21: Alokasi Disk Manual

Lakukan alokasi disk secara manual dengan memilih "custom storage layout" arahkan kursor tekan "space" di keyboard.


## Langkah 22: Tambah Partisi Root

Kemudian pilih free space di storage configuration dan pilih "add gpt partition".
![Screenshot_19](https://github.com/user-attachments/assets/70ad3cb9-8924-46c8-a8ba-ac2f0e47409c)



Pilih 7 GB untuk alokasi root dengan format ext4 dan mount "/".
![Screenshot_20](https://github.com/user-attachments/assets/816ca07e-9549-4878-923d-d20f3aca693d)



## Langkah 23: Tambah Partisi Swap

Ulang sebelumnya yaitu pilih 2,8 GB untuk alokasi swap dengan memilih format swap.
![Screenshot_21](https://github.com/user-attachments/assets/8d5a5f5d-3337-46e6-887f-2ffafbe94495)


## Langkah 24: Selesaikan Alokasi Disk

Pilih done kemudian tetap lanjutkan instalasi.
![Screenshot_22](https://github.com/user-attachments/assets/f138844d-bf34-4e66-8aef-af6c66ffa868)
![Screenshot_23](https://github.com/user-attachments/assets/ca09af74-74db-4a4b-9c73-1e283c1103d4)


## Langkah 25: Atur Profil

Kemudian atur profile configuration sesuai dengan kebutuhan.
![Screenshot_24](https://github.com/user-attachments/assets/d18a593b-2cd0-485c-a916-471c15c85802)

## Langkah 26: Lewati Upgrade Ubuntu Pro

Saat muncul "upgrade to Ubuntu Pro" dapat di skip.
![Screenshot_25](https://github.com/user-attachments/assets/604a2137-5273-4b32-8eed-b015c4b7609c)


## Langkah 27: Lewati Konfigurasi SSH

Kemudian muncul "ssh configuration" dapat di skip.

## Langkah 28: Lewati Fitur Server Snap

Untuk feature server snap juga dapat di skip.

## Langkah 29: Tunggu Instalasi Selesai

Tunggu proses installasi Ubuntu Server
![Screenshot_26](https://github.com/user-attachments/assets/fde3c0f4-7a2b-48c8-ae02-84c3b9a82a34)


## Langkah 30: Reboot Server

Pilih reboot now untuk merestart Ubuntu Server
![Screenshot_27](https://github.com/user-attachments/assets/53b452e2-30bf-4041-9956-e28b7c659dd8)


## Langkah 31: Login

Lakukan login dengan user yang sudah dibuat sebelumnya.
![Screenshot_28](https://github.com/user-attachments/assets/9404a7c2-6541-403a-9b2c-039d03ca17f9)


## Langkah 32: Cek Koneksi Internet

Lakukan pengecekan internet dengan prompt `ping 8.8.8.8` atau `ping google.com` apabila terhubung cancel dengan menekan `ctrl+c`.
![Screenshot_29](https://github.com/user-attachments/assets/33520c16-4892-46f0-8336-b14d369d08ee)


## Langkah 33: Update Paket

Lakukan prompt `sudo apt update`.
![Screenshot_30](https://github.com/user-attachments/assets/3374c0ea-d34a-461d-966d-cf2025d6b32a)


## Langkah 34: Instalasi Selesai

Instalasi sudah selesai.

---

### TASK 3
