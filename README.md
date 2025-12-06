1. Analisis Jumlah Siswa Mengulang di SD Kota Makassar Tahun 2024

Proyek ini bertujuan untuk menganalisis data jumlah siswa yang mengulang kelas di Sekolah Dasar (SD) Kota Makassar tahun 2024, serta membangun model machine learning sederhana untuk mengelompokkan tingkat risiko berdasarkan data pengulangan siswa. Proyek ini mengikuti standar proses CRISP-DM, meliputi pemahaman bisnis, pengolahan data, pemodelan, evaluasi, dan deployment menggunakan Gradio.

3. Tujuan Proyek
   - Mengidentifikasi kecamatan atau sekolah dengan persentase siswa mengulang yang tinggi.
   - Mengelompokkan sekolah ke dalam kategori risiko: Rendah, Sedang, dan Tinggi.
   - Membangun model machine learning sederhana untuk memprediksi risiko berdasarkan data kecamatan.
   - Menyediakan aplikasi Gradio untuk mempermudah penggunaan model.

4. CRISP-DM Overview
   1) Business Understanding
      Memahami permasalahan tingginya jumlah siswa mengulang kelas di beberapa kecamatan dan kebutuhan untuk mengidentifikasi risiko berdasarkan data.
   2) Data Understanding
      Data berasal dari file Excel yang memuat nama sekolah, kecamatan, dan jumlah siswa mengulang per tingkat kelas (Kelas 1–6).
   3) Data Preparation
      - Menghapus kolom kosong (Unnamed).
      - Menangani nilai kosong.
      - Membuat fitur baru: Total_Mengulang dan Risk_Category.
      - Melakukan OneHotEncoding pada kecamatan.
   4) Modeling
      Menggunakan Random Forest Classifier untuk memprediksi kategori risiko.
   5) Evaluation
      - Model diuji menggunakan accuracy, precision, recall, dan F1-score
      - Namun hasil akurasi 100% disebabkan oleh kurangnya variasi label (dataset hanya berisi kategori "Rendah").
