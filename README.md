# Tugas Praktikum: Aplikasi Dice Roller (Jetpack Compose)

Repositori ini dibuat untuk memenuhi tugas praktikum mata kuliah Pemrograman Perangkat Bergerak mengenai dasar-dasar interaktivitas menggunakan Jetpack Compose pada Android Studio.

---

## 👤 Identitas Mahasiswa
* **Nama:** Abdullah Tsaqif Cakrawibowo
* **NIM:** 452024611036
* **Kelas:** TI 5 A1
* **Proyek:** Aplikasi Dice Roller (Google Developer Codelab)

---

## 🛠️ Konsep & Fitur yang Diimplementasikan

Sesuai dengan instruksi modul Codelab dan rubrik tugas, aplikasi ini telah mengimplementasikan beberapa konsep utama Jetpack Compose:

### 1. Tata Letak (Layout) Dasar
* Menggunakan komponen **`Column`** untuk menyusun tata letak secara vertikal. Elemen gambar dadu (`Image`) dan tombol (`Button`) tersusun rapi dari atas ke bawah dan diposisikan di tengah layar menggunakan `Alignment.CenterHorizontally` dan `wrapContentSize(Alignment.Center)`.
* Menggunakan **`Spacer`** untuk memberikan jarak estetika antara gambar dadu dan tombol pelempar.

### 2. State Management (Re-composition)
* Menerapkan **`remember { mutableStateOf(1) }`** untuk menyimpan status (state) nilai dadu. Komponen ini memastikan bahwa setiap kali tombol ditekan dan nilai dadu berubah, antarmuka pengguna (UI) akan melakukan *re-composition* dan langsung memuat gambar dadu yang baru tanpa kehilangan data sebelumnya.

### 3. Logika Acak (Randomizer) & Event Handler
* Menggunakan fungsi bawaan Kotlin **`(1..6).random()`** di dalam aksi ketukan tombol (`onClick`). Fungsi ini menghasilkan angka acak dari 1 hingga 6.
* Menggunakan percabangan kondisional (`when`) untuk memetakan hasil angka acak secara dinamis ke aset visual resmi yang ada di folder `res/drawable` (dari `dice_1.xml` hingga `dice_6.xml`).

---

## 📈 Progres Riwayat Git (Commit History)
Proyek ini dikerjakan secara bertahap menggunakan *version control* Git dengan riwayat *commit* sebagai berikut:
1. `feat: susun layout dan asset dadu` (Fase penyiapan struktur awal aplikasi dan pengunggahan aset gambar dadu).
2. `feat: implementasi logika acak dan state` (Fase penambahan fungsi tombol, State Compose, dan logika acak 1-6).

---
