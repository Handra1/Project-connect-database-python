# Project-connect-database-python
This project about learning connecting to database in python (In Indonesia)

Python memiliki banyak tools yang dapat kita gunakan untuk database. Salah satunya adalah SQLAlchemy yang akan kita pelajari pada materi kali ini.
SQLAlchemy mengijinkan kita untuk men-generate query SQL yang kita tuliskan pada script Python. Maka dari itu pastikan teman - teman sudah pernah belajar atau paham tentang penulisan query SQL dengan baik.

SQLAlchemy memiliki 2 komponen utama. Yaitu:

- Core (Relational Modul focused)
- ORM (User Data Modul focused)

Terdapat banyak perbedaan tipe database dan masing - masing tipe memiliki keunikan dan kemampuan yang berbeda. Seperti SQLite, PostgreSQL, MySQL, Microsoft SQL Server, Oracle, dll.
SQLAlchemy menyediakan operasi untuk berbagai tipe database secara konsisten. Untuk bisa terkoneksi dengan database, yang kita perlukan adalah sebuah engine sebagai common interface.

Untuk membuat engine kita perlu meng-import fungsi create_engine dari sqlalchemy.
Kemudian gunakan fungsi engine dan membuat connection string ke database. File yang digunakan adalah file census.sqlite. SQLAlchemy tidak akan membuat koneksi hingga kita membuat perintah untuk execute program.
Kesimpulannya adalah engine adalah antarmuka umum (common interface) ke database, yang membutuhkan string koneksi untuk memberikan detail yang digunakan untuk menemukan dan terhubung ke database.
sqlite menunjukan: Driver + Dialect.
census.sqlite menunjukan: nama file yang ada di direktori.
Menggunakan method table_name() untuk melihat daftar tabel yang ada di dalam database itu.
Selanjutnya setelah mengetahui tabel apa saja yang ada di database, kita perlu mempunyai akses untuk mengolah tabel tersebut. Untuk melakukan itu maka kita perlu sebuah proses yang disebut reflection. Reflection adalah proses untuk dapat membaca database dan membuat objek tabel.
Disini kita gunakan fungsi repr() untuk melihat informasi detail dari tabel yang disimpan dengan nama census.
