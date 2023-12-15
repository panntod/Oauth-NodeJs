# OAuth Google 2.0

## Deskripsi

Dalam repo ini, mengimplementasikan OAuth atau outentikasi menggunakan layanan dari google (versi 2.0), dan setelah berhasil login maka akan menampilkan sebuah web todolist sederhana yang menyimpan data menggunakan MongoDB dan menggunakan materialize untuk membuat tampilan website lebih menarik
## Fitur

- Sistem CRUD
- Akses MongoDB
- Rest API
- OAuth Google (v2.0)

## Cara Membuat Aplikasi

### Langkah 1: 

Pastikan sudah membuat OAuth Google Project atau buat menggunakan link ini:

[Google Cloud Console](https://console.cloud.google.com/projectselector2/apis/credentials/consent?supportedpurview=project).

### Langkah 2: 

setelah itu masukan token api yang telah didapatkan ke dalam ```passport.js```
```js
 {
        clientID: process.env.GOOGLE_CLIENT_ID,
        clientSecret: process.env.GOOGLE_CLIENT_SECRET,
        callbackURL: "/auth/google/callback",
  },
```

### Langkah 3: 

Jalan kan perintah ini untuk mendapatkan package:
```
npm install
```
