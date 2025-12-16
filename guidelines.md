# Annotation Guidelines – Indonesian Text Annotation

## Objective
Menafsirkan dokumen berbahasa Indonesia dan mengekstraksi informasi penting ke dalam format terstruktur (JSON) secara konsisten dan akurat.

## Jenis Dokumen
Dokumen publik berbahasa Indonesia seperti:
- Pengumuman
- Deskripsi pekerjaan
- Informasi program
- Informasi layanan organisasi

## Skema Data
Setiap dokumen akan dikonversi ke dalam struktur berikut:

- judul_dokumen
- organisasi
- jenis_dokumen
- lokasi
- tanggal
- informasi_penting

## Definisi Field
- judul_dokumen: Judul atau topik utama dokumen.
- organisasi: Nama instansi, perusahaan, atau penyelenggara.
- jenis_dokumen: Kategori dokumen (contoh: lowongan kerja, pengumuman, program).
- lokasi: Lokasi yang disebutkan secara eksplisit (kota, provinsi, atau nasional).
- tanggal: Tanggal yang tertulis dalam dokumen (jika ada).
- informasi_penting: Poin-poin informasi utama yang relevan.

## Aturan Umum
- Jika informasi tidak disebutkan secara eksplisit, isi dengan "unknown".
- Jangan menebak atau menyimpulkan informasi.
- Gunakan bahasa Indonesia sesuai teks asli.
- Informasi ditulis secara ringkas namun lengkap.

## Penanganan Ambiguitas
- Jika lokasi tidak jelas → lokasi = "unknown"
- Jika tanggal tidak disebutkan → tanggal = "unknown"
- Jika terdapat lebih dari satu informasi penting → pisahkan dalam bentuk list

