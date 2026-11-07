# Day-1-FC27_NadyaMutiaraSani
**Nama Lengkap: Nadya Mutiara Sani**

## Deskripsi singkat mengenai repository:
Repository ini saya buat untuk menyimpan hasil dan catatan dari workshop "Building with AI, Managing Change with GitHub". Isinya ada dokumentasi kegiatan workshop dan proyek Student Task Planner yang dibuat di Day 1.

## Tujuan atau kegunaan Repository
1. Menyimpan catatan dan dokumentasi workshop supaya gampang dibuka lagi kalau lupa materinya.
2. Tempat latihan memakai Git dan GitHub, seperti `git init`, `git add`, `git commit`, dan `git push`.
3. Menyimpan proyek Student Task Planner yang dibuat dengan bantuan AI, sekaligus mencatat perubahan-perubahannya.

# Dokumentasi Workshop Day 1
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/645c87f9-ae74-4fbc-ab70-e4b00b6b2eea" />
<img width="720" height="1280" alt="image" src="https://github.com/user-attachments/assets/4fa8d034-c500-43d1-a526-6b9364b0c475" />

## 1. Rangkuman Materi
Workshop hari pertama dibagi jadi dua bagian besar. Bagian pertama tentang cara membuat dan mengembangkan sesuatu dengan AI, bagian kedua tentang cara mengelola perubahan dan kerja bareng pakai Git dan GitHub.

### Prompt Engineering
Prompt itu instruksi yang kita kasih ke AI supaya dia ngasih hasil yang kita mau. Bentuknya bisa pertanyaan biasa, kata kunci, atau instruksi yang panjang. Kata pemateri, prompt engineering adalah cara menyusun instruksi supaya jawaban AI tepat, relevan, dan layak dipakai. Di slide ada contoh perbandingan. Prompt "Create student task planner" saja hasilnya pasti kurang jelas, karena AI tidak tahu aplikasinya buat siapa dan fiturnya apa. Kalau prompt-nya dikasih konteks (misalnya untuk mahasiswa tahun pertama, harus ada daftar tugas, filter, dan tampilan responsif), hasilnya jauh lebih sesuai.

Struktur prompt yang bagus ada empat bagian:
1. Role: AI diminta berperan sebagai apa.
2. Task: tugas atau tujuan yang mau dicapai.
3. Context: kebutuhan (requirements) dan batasan (constraints).
4. Format: bentuk hasil yang diminta, misalnya kode lengkap tiap file dan cara menjalankannya.
Ada juga beberapa taktik dari contoh slide, seperti pakai kata kerja yang jelas, tentukan panjang dan format hasil, sebutkan target pembaca, kasih fakta atau data, dan rujuk dokumen tertentu. Keuntungannya: performa AI lebih baik, bias dan respons yang tidak pantas berkurang, hasil lebih bisa dikontrol dan diprediksi, dan pengalaman memakai AI jadi lebih enak.

### Git dan GitHub
Git adalah version control system yang mencatat siapa, kapan, dan apa saja yang berubah di sebuah file. Git dibuat oleh Linus Torvalds tahun 2005. Git berjalan di komputer kita (lokal). Sedangkan GitHub adalah platform berbasis web untuk menyimpan repository Git secara online dan dipakai untuk kolaborasi.

Alur kerja Git ada tiga tempat:
1. Working directory: folder proyek yang sedang kita kerjakan di komputer.
2. Staging area: tempat file yang sudah dipilih untuk masuk ke commit berikutnya.
3. Git directory (repository): tempat Git menyimpan semua riwayat dan data proyek.

Perintah dasar yang dipelajari:
1. `git init` untuk memulai repository baru
2. `git add .` untuk memindahkan file ke staging area
3. `git commit -m 'message'` untuk menyimpan perubahan ke repository
4. `git remote add <name> <url>` untuk menghubungkan repository lokal ke GitHub
5. `git push origin main` untuk mengirim perubahan ke GitHub
6. `git pull origin main` untuk mengambil perubahan dari GitHub
7. `git clone "url"` untuk menyalin repository dari GitHub

### Setup
Langkah setup yang dilakukan: install Git lalu cek dengan `git --version`, atur identitas dengan `git config --global user.name` dan `user.email`, install VS Code, lalu buat SSH key dengan `ssh-keygen -t ed25519`. Public key-nya ditambahkan ke pengaturan SSH and GPG keys di GitHub, lalu koneksi dicek dengan `ssh -T git@github.com`. Kalau berhasil, muncul pesan bahwa kita sudah berhasil terautentikasi.

### Praktik: Student Task Planner
Di akhir sesi kami membuat aplikasi sederhana bernama Student Task Planner. Urutannya: siapkan platform AI, tulis prompt untuk membuat aplikasinya, jalankan `git init`, commit dan push ke GitHub, lalu coba ubah sesuatu dan commit dan push lagi.

## 2. Poin Penting dan Pengetahuan Baru
1. Prompt yang singkat dan asal biasanya menghasilkan jawaban yang asal juga. Makin jelas konteksnya, makin bagus hasil dari AI.
2. Prompt yang rapi bisa disusun dengan pola Role, Task, Context, dan Format.
3. Di prompt contoh ada kalimat supaya AI tidak bilang aplikasinya jalan sebelum dicek. Ini baru saya sadari penting, karena hasil AI tetap harus kita cek sendiri.
4. Git dan GitHub itu beda. Git itu alatnya di komputer kita, GitHub itu tempat menyimpannya di internet.
5. Sebelum di-commit, file harus masuk staging area dulu. Jadi alurnya working directory, staging area, lalu repository.
6. `git add .`, `git add -A`, dan `git add *` kelihatannya mirip tapi tidak persis sama. Yang `*` tidak ikut menambahkan file yang dihapus.
7. Sebelum memakai Git, identitas (nama dan email) harus diatur dulu supaya riwayat perubahan ada nama pembuatnya.
8. SSH key dipakai supaya kita bisa terhubung ke GitHub dengan aman tanpa login terus-menerus. Passphrase boleh diisi atau dikosongkan.
9. Commit dan push sebaiknya dilakukan setiap kali ada perubahan, jadi kalau ada masalah kita masih punya versi sebelumnya.

## 3. Pendapat Pribadi tentang Day 1
Menurut saya Day 1 ini seru dan berguna banget, terutama buat saya yang masih mahasiswa baru. Sebelumnya saya cuma tahu AI buat tanya-tanya, ternyata cara menulis prompt-nya berpengaruh besar ke hasilnya. Contoh perbandingan prompt pendek dan prompt panjang di slide membuat saya langsung paham bedanya. Untuk bagian Git dan GitHub, awalnya saya agak bingung dengan istilah seperti staging area, commit, dan push. Tapi setelah ada gambar alurnya dan dicoba langsung lewat terminal, jadi lebih kebayang. Bagian yang menurut saya paling ribet itu setup SSH key, karena langkahnya banyak dan harus teliti, salah sedikit bisa gagal terhubung.
