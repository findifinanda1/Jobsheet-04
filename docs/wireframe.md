+--------------------------------------+
|             SIMPUS-Mini              |
|--------------------------------------|
|                                      |
|           [ Login Petugas ]          |
|                                      |
|   Username     : [______________]    |
|   Password     : [______________]    |
|                                      |
|                                      |
|                                      |
|               [ Masuk ]              |
|                                      |
|   Sudah punya akun? Login di sini    |
+--------------------------------------+


+-------------------------------------------+
|            SIMPUS-Mini               	  |
|-------------------------------------------|
|                                      	  |
|      [ Registrasi Anggota Baru ]     	  |
|                                           |
|   Nama Lengkap : [___________]            |
|   Alamat       : [___________]    	  |
|   No. Telepon  : [___________]            |
|   Email        : [___________]            |
|                                      	  |
|   [ Daftar ]        	[ Batal ]        	  |
|                                      	  |
|   Sudah punya akun? Login di sini         |
+--------------------------------------------+

// UserFlow Petugas Mencari Anggota dengan Tunggakan Lewat Jatuh Tempo

[Petugas Login]
      |
      v
[Dashboard]
      |
      v
[Klik menu "Anggota"]
      |
      v
[Halaman Daftar Anggota tampil]
      |
      v
[Pilih filter "Tunggakan Terlambat"]
      |
      v
[Sistem mengecek: ada anggota yang terlambat?]
      |
      +-- Ya ----> [Tampil daftar anggota bertunggakan]
      |                      |
      |                      v
      |            [Klik salah satu anggota]
      |                      |
      |                      v
      |            [Lihat detail: buku yang dipinjam,
      |             tanggal jatuh tempo, lama terlambat]
      |                      |
      |                      v
      +-- Tidak -> [Tampil pesan "Tidak ada anggota bertunggakan"]
                             |
                             v
                   [Kembali ke Dashboard]

