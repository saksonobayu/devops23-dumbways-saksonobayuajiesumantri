# NodeJS
- Deploy app wayshub-frontend
- Berjalan di port 3000
- Menggunakan NodeJS 13

**1. Instalasi node js di official website https://nodejs.org/en/download**
> ganti kebutuhan versi dengan versi 13, untuk linux, menggunakan nvm, dengan npm

![Screenshot_1](./images/Screenshot_25.png)

**2. Melakukan instalasi sesuai petunjuk yang ada di atas**
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash
```

![Screenshot_1](./images/Screenshot_1.png)

**3. Melakukan perintah exec bash agar sistem mendeteksi perintah node js atau update path**
```bash
exec bash
```

![Screenshot_1](./images/Screenshot_2.png)

**4. Melakukan restart shell**
```bash
\. "$HOME/.nvm/nvm.sh"
```

![Screenshot_1](./images/Screenshot_3.png)

**5. Melakukan instalasi node js versi 13**
```bash
nvm install 13
```

![Screenshot_1](./images/Screenshot_21.png)

**6. Memberi akses ke port 3000**
```bash
sudo ufw allow 3000
```
```bash
sudo ufw status
```

![Screenshot_1](./images/Screenshot_27.png)

**7. Melakukan git clone wayshub-frontend**
```bash
git clone git@github.com:dumbwaysdev/wayshub-frontend.git
```

![Screenshot_1](./images/Screenshot_35.png)

**8. Masuk ke direktori wayshub-frontend**
```bash
cd wayshub-frontend
```

![Screenshot_1](./images/Screenshot_36.png)

**9. Menggunakan npm versi 13**
```bash
nvm use 13
```

![Screenshot_1](./images/Screenshot_37.png)

**10. Melakukan perintah npm start untuk deploy project wayshub-frontend**
```bash
npm start
```

![Screenshot_1](./images/Screenshot_38.png)
* nah disitu terdapat error karena dependency nya belum ada, maka install dengan npm install

```bash
npm install
```

**11. Buka browser dan akses ip address dengan port 3000**
```bash
192.168.100.200:3000
```

![Screenshot_1](./images/Screenshot_39.png)
![Screenshot_1](./images/Screenshot_40.png)

# Python
- Deploy app menampilkan text nama kalian!
- Berjalan di port 5000 & bisa dibuka melalui web

**1. Melakukan instalasi pip yaitu package untuk python**
```bash
sudo apt install python3-pip
```
![Screenshot_1](./images/Screenshot_28.png)

**2. Membuat direktori python biar rapi gitu aja**
```bash
mkdir python
```
![Screenshot_1](./images/Screenshot_29.png)

**3. Instalasi library flask**
```bash
pip install flask
```
![Screenshot_1](./images/Screenshot_30.png)

**4. Membuat file index.py di dalam direktori python dan copy snippet code berikut**
```bash
cat > index.py
from flask import Flask

app = Flask(__name__)

@app.route('/')
def index():
    return 'SAKSONO BAYU AJIE SUMANTRI!'

app.run(host='0.0.0.0', port=5000)
```

![Screenshot_1](./images/Screenshot_31.png)

**5. Memberi akses port 5000**
```bash
sudo ufw allow 5000
sudo ufw status
```
![Screenshot_1](./images/Screenshot_32.png)

**6. Eksekusi python dengan python3 index.py kemudian copy address ke web**
```bash
python3 index.py
```
![Screenshot_1](./images/Screenshot_33.png)
![Screenshot_1](./images/Screenshot_34.png)

# Golang
- Deploy app menampilkan text "Golang geming!"

**1. Instalasi version golang dari official website https://go.dev/dl/**
```bash
wget https://go.dev/dl/go1.24.2.linux-amd64.tar.gz
```

![Screenshot_1](./images/Screenshot_41.png)

**2. Menjadi super user untuk install golang https://go.dev/doc/install**
```bash
sudo su
rm -rf /usr/local/go && tar -C /usr/local -xzf go1.24.2.linux-amd64.tar.gz
```

![Screenshot_1](./images/Screenshot_42.png)

**3. Export golang ke path environment**
```bash
export PATH=$PATH:/usr/local/go/bin
```

![Screenshot_1](./images/Screenshot_43.png)

**4. Mengecek versi**
```bash
go version
```

![Screenshot_1](./images/Screenshot_44.png)

**5. Membuat direktori golang biar rapi dan buat file index.go**
```bash
mkdir golang
cd golang
nano index.go
```

![Screenshot_1](./images/Screenshot_46.png)

* nah kemudian copy snipet code ke dalam file index.go
```bash
package main

import (
	"fmt"
	"net/http"
)

func handler(w http.ResponseWriter, r *http.Request) {
	fmt.Fprintf(w, "<h1>Golang Geming</h1>")
}

func main() {
	http.HandleFunc("/", handler)
	fmt.Println("Server running on http://192.168.1.1:8080...")
	http.ListenAndServe("192.168.100.200:8080", nil)
}
```

![Screenshot_1](./images/Screenshot_45.png)

**6. Jangan lupa kasih akses ke port 8080**
```bash
sudo ufw allow 8080
```

![Screenshot_1](./images/Screenshot_47.png)


**7. Eksekusi golang dengan perintah berikut**
```bash
go run index.go
```

![Screenshot_1](./images/Screenshot_49.png)

**8. Buka browser dan akses ip addressnya**
```bash
192.168.100.200:8080
```

![Screenshot_1](./images/Screenshot_48.png)


