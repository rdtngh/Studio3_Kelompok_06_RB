# Studio Proyek 3 – Fine-Tuning Transformer untuk NLP

Tugas kelompok mata kuliah Pembelajaran Mendalam (IF25-40401), Program Studi Teknik Informatika, Institut Teknologi Sumatera.

## Anggota Kelompok 6

- Raditya Alrasyid Nugroho (123140125)
- Bening Apni Prameswari (123140089)

## Deskripsi

Proyek ini membandingkan performa dan efisiensi model Transformer pretrained untuk klasifikasi sentimen teks Bahasa Indonesia menggunakan dataset SmSA (IndoNLU). Sentimen diklasifikasikan menjadi tiga kelas, yaitu positif, netral, dan negatif.

## Rancangan Eksperimen

Backbone yang digunakan:

- Multilingual BERT (mBERT)
- DistilBERT
- IndoBERT

Strategi fine-tuning:

- Full Fine-Tuning
- Partial Freezing
- Linear Probing

Setiap kombinasi diuji menggunakan tiga random seed sehingga menghasilkan total 27 run eksperimen. Seluruh eksperimen dilakukan menggunakan satu notebook Google Colab dengan GPU Tesla T4.

## Evaluasi

Perbandingan dilakukan berdasarkan Accuracy, Macro F1, waktu pelatihan, waktu inferensi, jumlah parameter total, jumlah parameter terlatih, dan penggunaan memori GPU. TF-IDF dengan Logistic Regression digunakan sebagai baseline.
