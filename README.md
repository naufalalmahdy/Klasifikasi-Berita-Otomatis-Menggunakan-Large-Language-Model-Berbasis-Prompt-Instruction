# Klasifikasi-Berita-Otomatis-Menggunakan-Large-Language-Model-Berbasis-Prompt-Instruction

## 🧠 Project Overview
### 🎯 Tujuan 
  Proyek ini bertujuan untuk membangun sistem klasifikasi berita otomatis menggunakan Large Language Model (LLM) berbasis prompt instruction. Sistem ini dirancang untuk mampu mengelompokkan berita ke dalam kategori utama seperti politik, ekonomi, teknologi, olahraga, kesehatan, dan hiburan tanpa memerlukan pelabelan manual atau pelatihan ulang model. Dengan memanfaatkan kemampuan LLM dalam memahami konteks dan bahasa alami, sistem ini diharapkan memberikan klasifikasi yang cepat, fleksibel, dan akurat terhadap berbagai topik berita.
### 📌 Latar Belakang
  Di era digital saat ini, produksi berita berlangsung dalam jumlah yang sangat besar setiap hari dari berbagai sumber dan platform. Hal ini menciptakan tantangan besar dalam mengelola, menyaring, dan mengkategorikan informasi secara efisien. Sistem klasifikasi otomatis menjadi sangat penting untuk:
- Menyajikan berita secara terstruktur kepada pengguna.
- Meningkatkan pengalaman pembaca melalui pengelompokan konten yang relevan.
- Mendukung sistem rekomendasi, pemilihan konten, dan analisis media.
### 🚩 Permasalahan Relevan
Kurangnya sistem klasifikasi yang fleksibel terhadap bahasa manusia dan konteks berita yang kompleks.
### 🛠️ Pendekatan
Proyek menggunakan LLM model ibm-granite-3.3-8b-instruct via Replicate untuk klasifikasi teks berita berbasis prompt-instruction.
## 🔗 Raw Dataset
Dataset berita diambil dari Kaggle: https://www.kaggle.com/code/gpreda/bbc-news-rss-feeds

## 💡 Insight & findings
### Politik
1. Ketegangan Geopolitik dan Konflik:
Artikel-artikel secara konsisten menyoroti sifat politis dari konflik Ukraina, dengan fokus pada hubungan internasional, tindakan pemerintah, dan implikasi geopolitik dari perang. Kategori "politik" muncul pada berita seperti "Kekacauan dan air mata saat ribuan orang mencoba naik kereta keluar dari Ukraina", "Peta Ukraina: Ukraina sebut tawaran gencatan senjata Rusia 'tidak bermoral'", dan "Berapa banyak pengungsi yang telah melarikan diri dari Ukraina dan ke mana mereka pergi?" — semua menunjukkan sudut pandang politik dalam pemberitaan.
2. Dampak terhadap Hubungan Internasional:
Artikel menunjukkan bagaimana perang memengaruhi politik global, termasuk hubungan diplomatik, sanksi internasional, dan strategi geopolitik para pemimpin dunia.
3. Krisis Kemanusiaan dan Respons Kebijakan:
Fokus pada pergerakan pengungsi dan upaya kemanusiaan menunjukkan keterkaitan antara keputusan politik dan dampaknya terhadap pengungsi serta integrasi mereka ke negara tujuan.

### Ekonomi
1. Dampak Ekonomi dari Perang:
Berita seperti "Lima cara perang Ukraina bisa menaikkan harga barang" menunjukkan keterkaitan langsung antara aksi militer dan indikator ekonomi seperti inflasi, harga energi, dan kenaikan biaya hidup.
2. Dampak Ekonomi Global:
Dampak ekonomi dari konflik ini meluas ke pasar global, harga komoditas, dan kebijakan ekonomi di banyak negara.
3. Reaksi Pasar Keuangan:
Berita seperti "Saham AS anjlok karena investor khawatir perlambatan ekonomi" menunjukkan bahwa ketidakpastian politik berdampak langsung pada pasar keuangan.

### Kesehatan
1. Dampak Psikologis dan Fisik:
Berita "Pemindaian otak menunjukkan bagaimana Covid dapat mengubah otak" menyoroti dampak jangka panjang Covid-19. Kasus seperti "Bayi tewas dalam serangan anjing di Ostler's Plantation" juga mencerminkan implikasi kesehatan dari insiden tragis.
2. Kesehatan Publik dan Respons Kebijakan:
Artikel yang membahas kebijakan kesehatan publik dalam menghadapi pandemi atau dampak kesehatan akibat konflik menunjukkan pentingnya sistem kesehatan yang tangguh dan responsif.

### Teknologi
1. Inovasi dan Adaptasi:
Berita seperti "Apple meluncurkan iPhone 14 dengan fitur kamera canggih" menunjukkan bagaimana industri teknologi terus berinovasi dan menyesuaikan diri dengan permintaan pasar.
2. Pengaruh Digital terhadap Hiburan:
Kasus "Ed Sheeran menyangkal tuduhan pelanggaran hak cipta lagu Shape of You di pengadilan" menggambarkan pertemuan antara teknologi, hukum, dan industri hiburan dalam konteks hak cipta digital.

## 🤖 AI Support Explanation
1. Peran AI (LLM)
LLM digunakan sebagai komponen utama klasifikasi tanpa pelatihan manual.
Model ibm-granite-3.3-8b-instruct dari Replicate dipilih karena kemampuannya memahami bahasa alami dan instruksi.
2. Cara AI Digunakan:
AI menerima prompt yang menyusun informasi (judul + deskripsi) lalu menghasilkan output kategori.
Parameter seperti temperature, top_k, dan max_tokens dikendalikan agar output konsisten dan relevan.

