<img width="1131" height="1600" alt="Revisi br" src="https://github.com/user-attachments/assets/a7932499-d1ea-459e-9d62-dcab04829fd0" />

## NAMA KELOMPOK :
## Rafi Ardian Saputra (1482500046)
## Muh Zaky Saifulloh Y (1482500057)
## Zaky Aksa Kafa Billah (1482500059)

# Sistem Pemesanan Tiket Bioskop

Sistem Pemesanan Tiket Bioskop merupakan aplikasi berbasis **Python** yang dikembangkan sebagai implementasi konsep **Object-Oriented Programming (OOP)**. Proyek ini menerapkan dua konsep utama OOP, yaitu **Encapsulation** dan **Polymorphism**, untuk menghasilkan sistem yang aman, terstruktur, fleksibel, dan mudah dikembangkan.

---

## Latar Belakang

Perkembangan teknologi informasi telah mengubah proses pemesanan tiket bioskop dari sistem manual menjadi sistem digital yang lebih cepat, efisien, dan mudah digunakan.

Melalui proyek ini dikembangkan sebuah sistem pemesanan tiket bioskop menggunakan bahasa pemrograman Python sebagai penerapan konsep **Object-Oriented Programming (OOP)**. Fokus utama sistem berada pada penerapan:

- **Encapsulation** untuk menjaga keamanan dan konsistensi data.
- **Polymorphism** untuk mengelola perhitungan harga berdasarkan jenis tiket.

---

## Tujuan

Proyek ini bertujuan untuk:

- Mengembangkan sistem pemesanan tiket bioskop berbasis Python.
- Menerapkan konsep **Encapsulation** pada setiap objek.
- Mengimplementasikan konsep **Polymorphism** dalam proses perhitungan harga.
- Menghasilkan aplikasi yang mudah dipahami, terstruktur, dan mudah dikembangkan.

---

## Alur Sistem

Alur kerja sistem adalah sebagai berikut:

1. Pengguna memasukkan data tiket:
   - ID Tiket
   - Judul Film
   - Nomor Kursi

2. Pengguna memilih jenis tiket:
   - Reguler
   - VIP
   - IMAX

3. Sistem menghitung harga tiket secara otomatis sesuai jenis tiket.

4. Informasi pemesanan ditampilkan beserta total pembayaran.

---

## Struktur Class

Sistem dibangun menggunakan konsep pewarisan (Inheritance) dengan struktur berikut.

```text
                    TiketBioskop
                 (Abstract Class)
                         │
        ┌────────────────┼────────────────┐
        │                │                │
TiketReguler      TiketVIP        TiketIMAX

                SistemPemesanan
          (Mengelola seluruh objek tiket)
```

---

## Implementasi Encapsulation

Konsep **Encapsulation** diterapkan pada class `TiketBioskop`.

Beberapa atribut penting dibuat sebagai atribut **private**, antara lain:

- ID Tiket
- Judul Film
- Nomor Kursi
- Harga Dasar

Akses data dilakukan menggunakan:

- Getter (`@property`)
- Setter dengan validasi data

Penerapan ini bertujuan untuk:

- Menjaga keamanan data
- Mencegah kesalahan input
- Menjamin konsistensi data

---

## Implementasi Polymorphism

Konsep **Polymorphism** diterapkan pada tiga class turunan:

- `TiketReguler`
- `TiketVIP`
- `TiketIMAX`

Setiap class mengimplementasikan method yang sama tetapi menghasilkan perilaku berbeda, yaitu:

```python
hitung_harga_akhir()
cetak_tiket()
```

Dengan pendekatan ini, sistem dapat memanggil method yang sama pada berbagai objek tanpa perlu mengetahui tipe class secara spesifik.

Keuntungan yang diperoleh:

- Program lebih fleksibel
- Mudah dikembangkan
- Kode lebih rapi
- Mengurangi duplikasi kode

---

## Implementasi Sistem

Seluruh proses pemesanan dikelola oleh class:

```text
SistemPemesanan
```

Class ini bertugas untuk:

- Menyimpan seluruh objek tiket
- Menambahkan data pemesanan
- Menampilkan seluruh data tiket
- Menghitung total pembayaran

Method utama yang digunakan:

```python
tambah_pesanan()
tampilkan_semua_tiket()
```

---

## Hasil Pengujian

Hasil pengujian menunjukkan bahwa sistem berhasil:

- Menambahkan data pemesanan.
- Mengelola berbagai jenis tiket.
- Menghitung harga sesuai jenis tiket.
- Menampilkan informasi tiket.
- Menghitung total pembayaran secara otomatis.

Implementasi **Encapsulation** dan **Polymorphism** berjalan sesuai dengan rancangan sistem.

---

## Pengembangan Selanjutnya

Beberapa pengembangan yang dapat dilakukan di masa mendatang:

- Menambahkan antarmuka berbasis GUI.
- Mengembangkan aplikasi berbasis web.
- Mengintegrasikan database.
- Menambahkan autentikasi pengguna.
- Menambahkan jadwal tayang film.
- Menambahkan pembayaran digital.
- Menyediakan fitur e-ticket.

---

## Teknologi

- Python
- Object-Oriented Programming (OOP)
- Encapsulation
- Polymorphism

---

## Konsep OOP yang Digunakan

- Abstract Class
- Inheritance
- Encapsulation
- Polymorphism
- Property
- Getter & Setter
- Method Overriding

---

## Kesimpulan

Sistem berhasil dikembangkan menggunakan bahasa pemrograman Python dengan menerapkan konsep **Object-Oriented Programming (OOP)**.

Penerapan **Encapsulation** menjaga keamanan dan konsistensi data melalui atribut private, getter, setter, serta validasi data. Sementara itu, **Polymorphism** memungkinkan setiap jenis tiket memiliki mekanisme perhitungan harga yang berbeda menggunakan method yang sama.

Seluruh fitur sistem berhasil berjalan sesuai rancangan, mulai dari proses input data, perhitungan harga, hingga menampilkan informasi pemesanan beserta total pembayaran.

---

## Dibuat Untuk

Tugas Mata Kuliah **Pemrograman Berorientasi Objek (PBO)**

Implementasi konsep:

- Encapsulation
- Polymorphism
- Object-Oriented Programming (OOP)

---

## Terima Kasih

Terima kasih telah mengunjungi repositori ini.

Semoga proyek ini dapat menjadi referensi pembelajaran mengenai penerapan konsep **Object-Oriented Programming (OOP)** menggunakan Python.
