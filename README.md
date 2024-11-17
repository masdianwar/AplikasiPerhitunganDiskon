# Aplikasi Kalkulator Diskon

## Deskripsi Program

Aplikasi ini adalah program GUI sederhana yang digunakan untuk menghitung harga akhir setelah diskon. Pengguna dapat memasukkan harga asli barang, memilih persentase diskon, serta memasukkan kode kupon untuk diskon tambahan. Program ini memberikan hasil berupa harga akhir setelah diskon dan jumlah penghematan.

### Fitur Utama
1. **Menghitung Harga Akhir:**
   - Pengguna memasukkan harga asli.
   - Memilih persentase diskon menggunakan `JComboBox` atau `JSlider`.
   - Hasil berupa harga akhir dan jumlah penghematan akan ditampilkan.

2. **Diskon Tambahan dengan Kode Kupon:**
   - Opsi untuk memasukkan kode kupon diskon tambahan.

3. **Riwayat Perhitungan:**
   - Menampilkan riwayat perhitungan diskon yang telah dilakukan selama sesi.

---


## Logika Program
1. **Perhitungan Diskon:**
   - Persentase diskon dipilih dari `JComboBox` atau `JSlider`.
   - Jika kode kupon diskon tambahan diisi, nilai diskon tambahan akan dihitung.
   - Harga akhir dihitung menggunakan formula:  
     \[
     \text{Harga Akhir} = \text{Harga Asli} \times (1 - (\text{Diskon Utama} + \text{Diskon Tambahan}))
     \]

2. **Penanganan Eksepsi:**
   - Validasi masukan seperti:
     - Memastikan harga asli adalah angka positif.
     - Memastikan format kode kupon valid (jika diimplementasikan).

3. **Riwayat Perhitungan:**
   - Menyimpan setiap hasil perhitungan dalam daftar (array atau `ArrayList`) untuk ditampilkan pada GUI.

---

## Events
1. **ActionListener untuk Tombol Hitung:**
   - Mengambil input dari `JTextField`, `JComboBox`, dan kode kupon.
   - Melakukan perhitungan diskon.
   - Menampilkan hasil perhitungan di GUI.

2. **ItemListener pada JComboBox:**
   - Menyesuaikan persentase diskon berdasarkan pilihan pengguna.

3. **ChangeListener untuk JSlider:**
   - Mengupdate nilai persentase diskon secara dinamis.

---
