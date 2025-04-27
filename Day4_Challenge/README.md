# 1. Repository dumbways-batch-23 dibuat private

* di halaman repositori saksono/dumbways-batch-23 pilih settings
![gambar1](./images/Screenshot_1.png)
  
* scroll paling bawah sampe ketemu danger zone kemudian pilih change visibility
![gambar1](./images/Screenshot_2.png)

* di dalam change visibility pilih change to private
  
![gambar1](./images/Screenshot_3.png)
  
* akan muncul popup seperti ini terus lanjutkan
  
![gambar1](./images/Screenshot_4.png)

![gambar1](./images/Screenshot_5.png)

![gambar1](./images/Screenshot_6.png)

# 2. Demokan penggunaan Pull Request
* clone repositori
```bash
git clone git@github.com:saksonobayu/dumbways-batch-23.git
```
![gambar1](./images/Screenshot_7.png)

* buat branch baru
```bash
git checkout -b main
```
![gambar1](./images/Screenshot_8.png)

* buat file di dalam branch baru
```bash
cat > kodenuklir.txt
```
```bash
snis41
```
![gambar1](./images/Screenshot_9.png)

* register file sebelum di commit
```bash
git add kodenuklir.txt
```
![gambar1](./images/Screenshot_10.png)

* commit file dengan deskripsi "commit di branch main"
```bash
git commit -m "commit di branch main"
```
![gambar1](./images/Screenshot_11.png)

* push file ke branch baru
```bash
git push -u origin main
```
![gambar1](./images/Screenshot_12.png)

* pull repositori dengan versi terakhir
```bash
git pull origin main
```
![gambar1](./images/Screenshot_13.png)

* mengambil semua folder dan file
```bash
git fetch --all
```
![gambar1](./images/Screenshot_14.png)

* menampilkan semua branch
```bash
git branch -a
```
![gambar1](./images/Screenshot_15.png)

