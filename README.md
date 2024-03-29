# OAuth Google 2.0 🌐

## Deskripsi

Dalam repo ini, mengimplementasikan OAuth atau autentikasi menggunakan layanan dari Google (versi 2.0). Setelah berhasil login, akan menampilkan sebuah web todolist sederhana yang menyimpan data menggunakan MongoDB dan menggunakan Materialize untuk membuat tampilan website lebih menarik.

## Fitur

- Sistem CRUD ✨
- Akses MongoDB 📊
- Rest API 🌐
- OAuth Google (v2.0) 🔐

## Cara Membuat Aplikasi

### Langkah 1:

Pastikan sudah membuat OAuth Google Project atau buat menggunakan link ini:

[Google Cloud Console](https://console.cloud.google.com/projectselector2/apis/credentials/consent?supportedpurview=project).

### Langkah 2:

setelah itu masukan token api yang telah didapatkan ke dalam `.env`

```env
 {
      PORT=3000
      MONGO_URI=<YourMongoUri>
      GOOGLE_CLIENT_ID=<YourToken>.apps.googleusercontent.com
      GOOGLE_CLIENT_SECRET=<YourToken>
  },
```

### Langkah 3:

dan digunakan untuk memproses `passport.js` untuk menyimpan data yang akan dikirim ke Google

```js
 {
        clientID: process.env.GOOGLE_CLIENT_ID,
        clientSecret: process.env.GOOGLE_CLIENT_SECRET,
        callbackURL: "/auth/google/callback",
  },
```

### Langkah 4:

Jalan kan perintah ini untuk mendapatkan package:

```
npm install
```
