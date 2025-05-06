# NodeJS + Python: Jalan di Background
**1. Instalasi library pm2**
```bash
npm install pm2 -g
```

![image](https://github.com/user-attachments/assets/6a500a13-08f7-4c75-b572-1d09fcd1a5bb)

**2. Masuk ke direktori nodejs dan run dengan pm2**
```bash
cd wayshub-frontend
```
```bash
pm2 start npm --name node.js -- start
```
![image](https://github.com/user-attachments/assets/e43eee6e-7312-4040-a88e-3bbfff90fd1d)

  
**3. Masuk ke direktori python dan run dengan pm2**
```bash
cd python
```
```bash
pm2 start index.py --name python --interpreter python3
```

![image](https://github.com/user-attachments/assets/764c754e-7036-46a0-bb6a-ba9ec3544bf2)




# Golang: Bisa Dibuka di Browser
**1. Jalankan Golang**
```bash
cd golang
go run index.go > go.log 2>&1 &
```

![Screenshot](./images/Screenshot_3.png)

![ezgif com-optimize](https://github.com/user-attachments/assets/fb9881bb-c0dd-42c5-a2f8-cd09f9163dd5)



