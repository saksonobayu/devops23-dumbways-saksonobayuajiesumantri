### STEP BY STEP PERINTAH LINUX
**1. Menuliskan perintah untuk update software linux**
```bash
sudo apt update
```
![Screenshot_1](https://github.com/user-attachments/assets/97a5d042-e10a-4d91-ac99-dbce51ead031)

**2. Menuliskan perintah untuk mengakses list perintah direktori**
```bash
mkdir --help
```
![Screenshot_3](https://github.com/user-attachments/assets/f2af1d7c-c584-44ff-93a6-c11a5fe7fe8e)

**3. Menuliskan perintah untuk membuat direktori dumbways dan perintah ls(list) untuk menampilkan folder yang sudah dibuat**
```bash
mkdir dumbways
```
```bash
ls
```
![Screenshot_4](https://github.com/user-attachments/assets/32f62a44-ee99-42d6-a4ed-882f5c259ed2)
![Screenshot_5](https://github.com/user-attachments/assets/0efa6eb0-b7cf-40e9-b096-aadc5af2c302)

**4. Menuliskan perintah untuk membuat file filesatu dan perintah ls(list) untuk menampilkan file yang sudah dibuat**
```bash
touch filesatu
```
![Screenshot_6](https://github.com/user-attachments/assets/c71f7c08-06f5-48a1-9d82-957a1cf78daf)

**5. Menuliskan perintah untuk menampilkan list dengan li dan la untuk menampilkan semua file termasuk yang hidden, dimana l adalah long format(detailed metadata) sedangkan a adalah all files**
```bash
ls -la
```
![Screenshot_7](https://github.com/user-attachments/assets/9a8d1337-3c71-4170-82e9-3cee7f1d2405)

**6. Menuliskan perintah untuk masuk ke direktori dumbways dan perintah untuk keluar dari direktori dumbways**
```bash
cd dumbways
```
```bash
cd ..
```
![Screenshot_8](https://github.com/user-attachments/assets/cebb0468-6c8c-4a5d-9b8e-d9d3d8ce33cc)

**7. Menuliskan perintah untuk copy file atau duplikat file, dimana filesatu adalah file yang akan di duplikat sedangkan sebelahnya adalah calon file duplikat dengan nama filedua**
```bash
cp filesatu filedua
```
![Screenshot_11](https://github.com/user-attachments/assets/ddb381ac-8bce-4d3e-82e6-a1c179581a89)

**8. Menuliskan perintah untuk move file atau memindahkan file, dimana filesatu dipindah ke dalam folder dumbways**
```bash
mv filesatu dumbways/filesatu
```
![Screenshot_12](https://github.com/user-attachments/assets/d2f9308a-9a9d-40c0-9184-db4a38f62c61)

**9. Menuliskan perintah untuk membuat text hello dumbways**
```bash
echo 'hello dumbways'
```
![Screenshot_13](https://github.com/user-attachments/assets/49440106-2acd-44ee-847e-acfdc6af3ce8)

**10. Menuliskan perintah untuk membuat text hello dumbways di dalam file.js**
```bash
echo 'hello dumbways' > file.js
```
**Menuliskan perintah untuk menampilkan text atau konten di dalam file.js**
```bash
cat file.js
```
**Menuliskan perintah untuk menampilkan text 2x dengan menambah simbol >>**
```bash
echo 'hello dumbways' >> file.js
```
![Screenshot_14](https://github.com/user-attachments/assets/ba519cb2-4e85-4cba-b348-afb677be9e7d)

**11. Menuliskan perintah find untuk mencari file atau folder, dengan catatan ini umum maka akan menampilkan semua file dan folder**
```bash
find
```
**perintah find dapat dibuat spesifik mencari folder atau file dengan prompt seperti ini**
```bash
find -type f
```
```bash
find -type d
```
```bash
find -type f -name filesatu
```
![Screenshot_15](https://github.com/user-attachments/assets/823637b9-7ccc-4b31-badd-d100a3bceadf)

**12. Perintah grep untuk mencari text atau input didalam file tertentu**
```bash
grep hello file.js
```
![Screenshot_16](https://github.com/user-attachments/assets/e6eff396-ea5e-400b-a848-b43034b17d2e)

**atau disemua file dengan menambah -r**
```bash
grep -r hello
```
![Screenshot_18](https://github.com/user-attachments/assets/d5b1ff87-54e1-4a5c-a4a1-898ff1d69bb2)


**13. Perintah untuk membuat text editor di dalam file.js**
```bash
nano file.js
```
![Screenshot_17](https://github.com/user-attachments/assets/34a32834-a331-4bb9-966e-474520a058ed)

**14. Perintah untuk mengubah permission file atau direktori**
```bash
chmod 777 file.js
```
```bash
chmod 773 file.js
```
![Screenshot_19](https://github.com/user-attachments/assets/422eb900-2ee1-40e6-aa78-8a383c6593da)

**15. Perintah untuk mengubah kepemilikan file atau direktori**
```bash
sudo chown root:root file.js
```
![Screenshot_20](https://github.com/user-attachments/assets/4cac9d81-d9c9-4c81-8653-44be358f91e7)

**16. Perintah untuk menampilkan riwayat semua perintah linux yang pernah dijalankan**
```bash
history
```
![Screenshot_21](https://github.com/user-attachments/assets/74328c72-550d-4b2f-b35c-6fc49b64a644)

**17. Perintah untuk menjadi super user**
```bash
sudo su
```
**perintah untuk keluar dari super user**
```bash
ctrl + x
```
![Screenshot_22](https://github.com/user-attachments/assets/d314083b-2730-421c-88b6-aaf61d1353b1)
![Screenshot_23](https://github.com/user-attachments/assets/789ac1a5-a5ce-4575-9ef3-c276afd367d1)
