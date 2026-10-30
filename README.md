# Tugas Flutter - Aplikasi Profil

Tugas mata kuliah Aplikasi Mobile (Pertemuan 5).

---

## Catatan Pengerjaan Hari 1

### 1. Hari 1 commit 1 - Bikin Kerangka Utama & Benerin Bug

- **Inisialisasi Root (`lib/main.dart`)**
  Pake `MaterialApp` buat root widget, atur warna tema ke deepPurple, terus set `home` ke `ProfilePage()`.

- **Bikin Halaman Profil (`lib/profile_page.dart`)**
  Menyusun kerangka tampilan awal pake `Scaffold` dan `AppBar`. Terus masang `CircleAvatar` sama `Column` buat nama & role di dalam `body`.

- **Perbaikan Bug Layout (Debugging)**
  - Munculin `import 'profile_page.dart';` biar nggak error.
  - Nambahin `Center()` sama `mainAxisAlignment` & `crossAxisAlignment` di `Column` biar ikon sama teksnya pas di tengah.
  - Ubah `SizedBox(width: 16)` jadi `SizedBox(height: 16)` biar dapet jarak vertikal yang pas.
  - Ubah isi variabel nama & role jadi data sendiri.

- **Pesan Commit:** `feat: create basic profile page structure with avatar and text`

---

### 2. Hari 1 commit ke 2 - Extract Widget (Bagian 1)

- **Refactoring UI**
  Memecah `Column` panjang di `profile_page.dart` jadi dua Custom Widget terpisah biar kodenya rapi dan bisa dipakai ulang.

- **Widget yang Dipisah**
  - `ProfileAvatar`: Khusus nampilin foto profil lingkaran.
  - `ProfileInfo`: Khusus nampilin teks nama dan role pake parameter passing data.

- **Pesan Commit:** `refactor: extract avatar and info into custom widgets`

### 3. Hari ke 2 commit ke 1 - Menambahkan btn dan membuat row
    * **Update Halaman Profil (`lib/profile_page.dart`)**
  * Nambahin **Tombol Edit Profil** pakai `ElevatedButton.icon` tepat di bawah info nama & role.
  * Nambahin widget **Row** untuk nampilin statistik profil (12, Proyek, Followers). 
  * Di sesi pagi ini, kodenya sengaja masih ditulis panjang dan ditumpuk manual (memakai 3 `Column` terpisah di dalam `Row`).

* **Pesan Commit:** `feat: add profile statistics row`

---

## Struktur File

```text
lib/
├── main.dart
└── profile_page.dart
```
