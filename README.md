# ♻️ SampahClassifier - Tahap Eksperimen & Preprocessing

Repositori ini merupakan **Bagian 1** dari rangkaian proyek sistem *Machine Learning Operations* (MLOps) untuk pengenalan citra jenis sampah daur ulang. Fokus utama repositori ini adalah membedah data mentah, melakukan eksplorasi, dan menyiapkan jalur prapemrosesan data yang bersih.

---

## 📂 Struktur Repositori

```text
Eksperimen_SML_Muhammad_Rahman/
├── .workflow/
│   └── main.yml                             # Salinan skrip GitHub Actions
├── preprocessing/
│   ├── Eksperimen_Muhammad_Rahman.ipynb     # Notebook untuk Exploratory Data Analysis (EDA)
│   ├── automate_Muhammad_Rahman.py          # Skrip otomatisasi pengunduhan & preprocessing dataset
│   └── sampah-daur-ulang_preprocessing/     # Folder wadah untuk dataset bersih
└── sampah-daur-ulang_raw/                   # Folder penampung dataset mentah
```

## 🛠️ Proses Preprocessing Data
1. **Pengunduhan Otonom:** Dataset ditarik secara terprogram melalui Kaggle API dari sumber `fathurrahmanalfarizy/sampah-daur-ulang`.
2. **Verifikasi Kualitas:** Mendeteksi dan mengeliminasi file gambar yang korup atau memiliki format *header* yang tidak valid.
3. **Standarisasi Dimensi:** Seluruh gambar di-*resize* ke standar resolusi masukan untuk arsitektur model *MobileNetV2*.

*Repositori ini dibuat sebagai pemenuhan Tugas Akhir kelas **Belajar Penerapan Machine Learning dengan MLOps** di Dicoding.*
