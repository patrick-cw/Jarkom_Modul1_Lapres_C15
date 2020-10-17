# Jarkom_Modul1_Lapres_C15
Lapres Modul 1 Jarkom

### Nama Anggota Kelompok :
### 1. Anggara Yuda Pratama (05111840000008)
### 2. Patrick (05111840000098)

### Display Filter
**1. Sebutkan webserver yang digunakan pada "testing.mekanis.me"!**
Mengisi display filter dengan : ```http.host contains "testing.mekanis.me"```

![1.1](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/1.1.png)

![1.2](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/1.2.png)

Lalu Follow TCP Stream, maka bisa dilihat server yang digunakan nginx/1.14.0 (Ubuntu)

**2. Simpan gambar "Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"!**
Mengisi display filter dengan : ```http contains "Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"```

![2.1](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/2.1.png)

Kemudian export objects → http, lalu save foto yang diminta

![2.2](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/2.2.png)

![2.3](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/2.3.png)

File yang didownload berada di komputer kita.

**3. Cari username dan password ketika login di "ppid.dpr.go.id"!**
Mengisi display filter dengan : ```http.host contains "ppid.dpr.go.id" && http.request.method ==  POST```

![3](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/3.png)

Lalu kita dapat melihat username & passwordnya untuk login di "ppid.dpr.go.id"

**4. Temukan paket dari web-web yang menggunakan basic authentication method!**
Mengisi display filter dengan : ```http.authbasic```

![4](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/4.png)

Lalu kita dapat melihat web-web dengan menggunakan Authorization yang basic.

**5. Ikuti perintah di aku.pengen.pw! Username dan password bisa didapatkan dari file .pcapng!**
Mengisi display filter dengan : ```http.host contains "aku.pengen.pw"```

![5.1](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/5.1.png)

Lalu kita mengisi pertanyaan yang ada di web "aku.pengen.pw"

![5.2](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/5.2.png)

**6. Seseorang menyimpan file zip melalui FTP dengan nama "Answer.zip". Simpan dan Buka file "Open This.pdf" di Answer.zip. Untuk mendapatkan password zipnya, temukan dalam file zipkey.txt (passwordnya adalah isi dari file txt tersebut).**

Mengisi display filter dengan : ```ftp-data```. Nanti mencari info yang "Answer.zip"

![6.1](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/6.1.png)

Klik kanan di info tersebut, follow -> TCP-Stream. Lalu ganti "Show and save data" as "Ascii" jadi "Raw.

![6.2](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/6.2.png)

Kemudian save as dengan nama file “Answer.zip”

![6.3](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/6.3.png)

Untuk mencari file yang berisi password, dengan mengisi display filter → ftp-data.
trus cari file dengan nama zipkey.txt. Kemudian follow → TCP Stream.

![6.4](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/6.4.png)

Lalu ketemu passwordnya

![6.5](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/6.5.png)

Setelah memasukkan password tersebut saat unzip, akan muncul isi file dari “Answer.zip” yaitu “Open This.pdf”

![6.6](https://github.com/anggarayp/Jarkom_Modul1_Lapres_C15/blob/main/Screenshots/6.6.png)

**7. Ada 500 file zip yang disimpan ke FTP Server dengan nama 1.zip, 2.zip, ..., 500.zip. Salah satunya berisi pdf yang berisi puisi. Simpan dan Buka file pdf tersebut.
Your Super Mega Ultra Rare Hint = nama pdf-nya "Yes.pdf"**

Mengisi display filter dengan : ```frame contains "Yes.pdf"```

