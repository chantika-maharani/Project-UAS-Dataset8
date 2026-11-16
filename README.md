# Proyek Akhir Pembelajaran Mesin (INF62325)
## Analisis Klastering Tingkat Obesitas Berdasarkan Kebiasaan Makan dan Aktivitas Fisik Menggunakan K-Means

### Anggota Kelompok
- **Chantika Maharani** (2488010080)  
*(Varian Pemilihan Fitur)*
- **Intan Fairuz Nur Asiyah** (2488010005)  
*(Varian Dasar)*
- **Tiara Salsabila** (2488010045)  
*(Varian Parameter / Perlakuan Data)*

**Kelas:** Informatika 5C

---

### Informasi Proyek
- **Paket Dataset:** Estimation of Obesity Levels Based On Eating Habits and Physical Condition
- **Metode:** K-Means Clustering (Metode 3)
- **Tautan Aplikasi:** [Masukkan Link Deploy Aplikasi di sini, misal: Streamlit Cloud / HuggingFace]
- **Repositori GitHub:** [Project-UAS-Dataset8-5C](https://github.com/chantika-maharani/Project-UAS-Dataset8)

---

### Deskripsi Dataset
Dataset yang digunakan berasal dari UCI Machine Learning Repository yaitu **Estimation of Obesity Levels Based On Eating Habits and Physical Condition**. Dataset ini mencakup data estimasi tingkat obesitas individu yang berasal dari negara Meksiko, Peru, dan Kolombia. Setiap baris data diberi label variabel target kelas `NObeyesdad` (tingkat obesitas) yang dikategorikan ke dalam tujuh tingkatan, mulai dari berat badan kurang hingga obesitas tipe III. Berdasarkan dokumentasi resminya, sekitar 77% data dibangkitkan secara sintetis menggunakan *tool* Weka dan filter SMOTE, sedangkan 23% sisanya dikumpulkan langsung dari responden melalui platform web.

Berdasarkan pemeriksaan mandiri melalui Google Colab:
- **Jumlah Baris (`df.shape`):** 2.111 baris (*records*)
- **Jumlah Kolom (`df.shape`):** 17 kolom (*attributes*)
- **Jumlah Nilai Kosong (`df.isnull().sum()`):** 0
- **Jumlah Baris Duplikat (`df.duplicated().sum()`):** 24 baris
- **Tautan Sumber Dataset:** [UCI Estimation of Obesity Levels Dataset](https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition)
- **Fitur yang Digunakan:** `FAVC`, `FCVC`, `CAEC`, `FAF`, dan `TUE`.

---

### Pertanyaan Analitik
> Ada berapa kelompok alami responden berdasarkan pola makan dan aktivitas, serta bagaimana masing-masing karakteristik kelompok yang terbentuk dengan menggunakan K-Means?

---

### Pembagian Varian Eksperimen
- **Intan Fairuz Nur Asiyah (Varian Dasar):** Membuat model klaster K-Means dasar menggunakan 5 fitur terpilih (`FAVC`, `FCVC`, `CAEC`, `FAF`, `TUE`) serta mengevaluasi sebaran klaster awalnya.
- **Tiara Salsabila (Varian Parameter / Perlakuan Data):** Melakukan uji coba penentuan jumlah klaster optimal ($k$) menggunakan Metode *Elbow* dan *Silhouette Score*, serta membandingkan hasil klaster sebelum dan sesudah penerapan *feature scaling*.
- **Chantika Maharani (Varian Pemilihan Fitur):** Membandingkan hasil pembentukan klaster K-Means dengan membedakan kombinasi subset fitur (misalnya membandingkan klaster yang dibentuk khusus dari fitur pola makan saja vs fitur aktivitas fisik), lalu menyusun profil serta penamaan tiap klaster.

---

### Cara Menjalankan Aplikasi & Notebook

#### 1. Prasyarat
Pastikan perangkat Anda sudah terinstal **Python 3.8+** dan **Git**.

#### 2. Clone Repositori
```bash
git clone [https://github.com/chantika-maharani/Project-UAS-Dataset8.git](https://github.com/chantika-maharani/Project-UAS-Dataset8.git)
cd Project-UAS-Dataset8