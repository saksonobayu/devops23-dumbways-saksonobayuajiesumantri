di halaman repositori saksono/dumbways-batch-23 pilih settings
scroll paling bawah sampe ketemu danger zone kemudian pilih change visibility
di dalam change visibility pilih change to private
akan muncul popup seperti ini terus lanjutkan

clone repositori
git clone git@github.com:saksonobayu/dumbways-batch-23.git

buat branch baru
git checkout -b main

buat file di dalam branch baru
cat > kodenuklir.txt
snis41

register file sebelum di commit
git add kodenuklir.txt

commit file dengan deskripsi "commit di branch main"
git commit -m "commit di branch main"

push file ke branch baru
git push -u origin main

pull repositori dengan versi terakhir
git pull origin main

mengambil semua folder dan file
git fetch --all
push

menampilkan semua branch
git branch -a


