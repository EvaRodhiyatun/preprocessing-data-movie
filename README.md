# preprocessing-data-movie

** Konteks **

Dalam industri perfilman, pemahaman yang mendalam tentang data film sangat penting untuk mendukung pengambilan keputusan, baik dari sisi produksi, distribusi, maupun strategi pemasaran. Informasi seperti anggaran produksi, pendapatan kotor, genre, sutradara, maupun skor penilaian dari penonton dapat memberikan wawasan berharga mengenai faktor-faktor yang mempengaruhi kesuksesan sebuah film. Oleh karena itu, penting untuk memiliki data yang bersih, konsisten, dan terstruktur agar analisis dapat dilakukan dengan akurat. Dataset Movie yang digunakan dalam penelitian ini berisi berbagai variabel terkait film, yang diolah sampai tahap preprocessing.

** Dataset **
Berikut adalah variabel-variabel yang terdapat dalam dataset.

** color ** : format warna film (misalnya Color atau Black and White)
** director_name ** : nama sutradara film
** duration ** : durasi film dalam menit
** gross ** : pendapatan kotor film
** genres ** : kategori atau jenis film (misalnya Action, Drama, Comedy)
** movie_title ** : judul film
** title_year ** : tahun rilis film
** language ** : bahasa utama yang digunakan dalam film
** country ** : negara asal produksi film
** budget ** : anggaran produksi film
** imdb_score ** : skor penilaian film berdasarkan IMDb
** actors ** : daftar aktor/aktris yang terlibat dalam film
** movie_facebook_likes ** : jumlah likes pada halaman Facebook film

** Langkah-langkah Preprocessing **
Berikut adalah langkah-langkah preprocessing dataset movie:

1.	Memuat Data
o	Import library yang diperlukan, seperti Pandas.
o	Muat dataset dari file CSV ke dalam DataFrame.
2.	Memeriksa Data
o	Tampilkan beberapa baris pertama dari dataset untuk memahami struktur data.
o	Periksa informasi umum tentang dataset, termasuk tipe data dan nilai yang hilang.
3.	Membersihkan Data
o	Hapus baris yang memiliki nilai NaN di kolom penting seperti gross dan budget.
o	Atasi nilai yang tidak konsisten atau kesalahan penulisan di kolom, seperti perbedaan antara "Color" dan "color".
o	Ubah atau hapus nilai-nilai yang tidak standar, seperti nilai negatif atau "N/A".
4.	Transformasi Data
o	Ubah tipe data kolom menjadi tipe data yang sesuai (misalnya, konversi budget dan gross menjadi numerik).
o	Pisahkan genre yang bergabung dalam satu kolom menjadi beberapa kolom terpisah (opsional).
o	Normalisasi teks untuk memastikan konsistensi (misalnya, mengubah teks menjadi huruf kecil).
5.	Penyimpanan Data
o	Simpan data yang telah diproses ke dalam file CSV baru dengan nama movie_dataset_cleaned.csv.
