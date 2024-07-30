# Improving Employee Retention by Predicting Employee Attrition Using Machine Learning
Project ini merupakan project yang bertujuan untuk meningkatkan retensi karyawan dengan memprediksi atrusi karyawannya. Project ini dibuat menggunakan bahasa pemrograman Python 

## Daftar Isi
- Data Preprocessing
- Laporan Tahunan Perubahan Jumlah Karyawan
- Analisis Alasan Mengundurkan Diri Untuk Strategi Manajemen Attrusi Karyawan
- Membangun Prediksi Perilaku Pengunduran Diri Otomatis Menggunakan _Machine Learning_
- Menyajikan Hasil _Machine Learning_ kepada Pengguna Bisnis

## Bagian 0: Pendahuluan
**1. Background** <br>
Sumber daya manusia (SDM) adalah aset utama yang perlu dikelola dengan baik oleh perusahaan agar tujuan bisnis dapat tercapai dengan efektif dan efisien. Pada kesempatan kali ini, kita akan menghadapi sebuah permasalahan tentang sumber daya manusia yang ada di perusahaan. Fokus kita adalah untuk mengetahui bagaimana cara menjaga karyawan agar tetap bertahan di perusahaan yang ada saat ini yang dapat mengakibatkan bengkaknya biaya untuk rekrutmen karyawan serta pelatihan untuk mereka yang baru masuk. Dengan mengetahui faktor utama yang menyebabkan karyawan tidak merasa, perusahaan dapat segera menanggulanginya dengan membuat program-program yang relevan dengan permasalahan karyawan.<br>

**2. Goals** <br>
Proyek ini bertujuan untuk mengatasi masalah kritis dari pengurangan karyawan dengan memanfaatkan machine learning. Retensi karyawan tidak hanya penting untuk kesejahteraan tenaga kerja, tetapi juga untuk keberhasilan dan stabilitas organisasi apapun.<br>

**3. Objective** <br>
Membuat visualisasi berbasis data sebagai insight bagi perusahaan, terutama HR

**4. Feature Description**
| Feature                            | Description                                                     |
|------------------------------------|-----------------------------------------------------------------|
| `Username`                           | Nama pengguna karyawan yang unik.                               |
| `EnterpriseID`                       | Identitas dalam perusahaan.                                     |
| `StatusPernikahan`                   | Status perkawinan.                                              |
| `JenisKelamin`                       | Jenis kelamin.                                                  |
| `StatusKepegawaian`                  | Status pekerjaan.                                               |
| `Pekerjaan`                          | Posisi pekerjaan.                                               |
| `JenjangKarir`                       | Tingkat karier.                                                 |
| `PerformancePegawai`                 | Peringkat kinerja.                                              |
| `AsalDaerah`                         | Wilayah asal.                                                   |
| `HiringPlatform`                     | Platform digunakan untuk menyewa.                               |
| `SkorSurveyEngagement`               | Skor pertunangan.                                               |
| `SkorKepuasanPegawai`                | Nilai kepuasan karyawan.                                        |
| `JumlahKeikutsertaanProjek`          | Jumlah proyek yang berpartisipasi.                              |
| `JumlahKeterlambatanSebulanTerakhir` | Hitungan keterlambatan bulanan terbaru.                         |
| `JumlahKetidakhadiran`               | Jumlah absen.                                                   |
| `NomorHP`                            | Nomor telepon karyawan.                                         |
| `Email`                              | Alamat email karyawan.                                          |
| `TingkatPendidikan`                  | Tingkat pendidikan.                                             |
| `PernahBekerja`                      | Riwayat pekerjaan sebelumnya.                                   |
| `IkutProgramLOP`                     | Partisipasi dalam program tertentu (LOP).                       |
| `AlasanResign`                       | Alasan pengunduran diri (jika berlaku).                         |
| `TanggalLahir`                       | Tanggal lahir.                                                  |
| `TanggalHiring`                      | Tanggal perekrutan.                                             |
| `TanggalPenilaianKaryawan`           | Tanggal evaluasi karyawan.                                      |
| `TanggalResign`                      | Tanggal pengunduran diri untuk karyawan yang mengundurkan diri. |

## Bagian 1: Data Preprocessing
Pada proses ini dilakukan pemrosesan data sekaligus pembersihan data, yang terdiri dari pemeriksaan null / missing value, duplikasi data, dan konsistensi nilai. Hasilnya tertera pada tabel dibawah.
![image](https://github.com/user-attachments/assets/9b418864-bb5f-4685-b242-eef2a4e7d691)

## Bagian 2: Laporan Tahunan Perubahan Jumlah Karyawan
Grafik dibawah menunjukkan tren perubahan jumlah karyawan dari tahun ke tahunnya.
![image](https://github.com/user-attachments/assets/37d7d3c2-c96b-437f-b2b1-5ec9ea6223f7)<br>
Berdasarkan grafik diatas, dapat dilihat bahwa:
1. Selama 2006-2013, jumlah karyawan yang masuk relatif rendah, dan ada peningkatan bertahap pada karyawan yang keluar.
2. Pada 2013, sejumlah besar karyawan mengundurkan diri, mengakibatkan penurunan tajam pada total karyawan yang tersisa. Tren ini berlanjut pada 2014 dan 2015. Peningkatan karyawan yang keluar mungkin disebabkan oleh berbagai faktor seperti ketidakpuasan pekerjaan, kesempatan kerja di tempat lain, dan lain sebagainya.
3. Jumlah karyawan yang masuk pada 2015-2017 tetap moderat, tetapi jumlah karyawan yang keluar tetap tinggi.
4. Pada 2018, jumlah karyawan yang masuk sangat rendah, sedangkan jumlah karyawan yang keluar secara signifikan lebih tinggi. Hal ini menyebabkan penurunan drastis pada total karyawan yang tersisa. Tren peningkatan pengunduran diri mungkin disebabkan oleh masalah internal atau faktor eksternal yang mempengaruhi stabilitas pekerjaan.

## Bagian 3: Analisis Alasan Mengundurkan Diri Untuk Strategi Manajemen Attrusi Karyawan
![image](https://github.com/user-attachments/assets/1f9f8348-5659-46e5-8307-9fd758f6c5f8)<br>
Terlihat bahwa Software Engineer adalah divisi yang paling dominan pada perusahaan dengan total 73,71% dari persentase dari seluruh divisi menunjukkan betapa pentingnya peran Software Engineer di perusahaan. Kemudian, divisi yang dominan diikuti oleh UI & UX dengan 7,73%, sementara divisi sisanya di bawah 6% menunjukkan beberapa asumsi bahwa ini mungkin ada beberapa hierarki struktural peran penting bagi perusahaan seperti Software Engineer.
![image](https://github.com/user-attachments/assets/b5dfa82a-5f38-4212-9a17-d4a1e9c5fade)<br>
Dapat terlihat bahwa karyawan yang resign paling banyak merupakan _fresh graduate_, diikuti dengan _mid level_ dan _senior level_ .
![image](https://github.com/user-attachments/assets/995d231e-2aa7-4924-a2ab-9a65e5f7ff83)<br>
Pada grafik ini, dapat terlihat bahwa pegawai yang _resign_ ternyata memiliki performa yang sangat bagus. Hal ini dapat disebabkan karena pegawai dituntut untuk mendapatkan kesempatan yang lebih baik atau tujuan pengembangan karier pribadi.
![image](https://github.com/user-attachments/assets/506468e2-ba8c-4803-865f-1dc48b4f00d0)<br>
Berdasarkan alasan resign, banyak pegawai yang mengajukan resign karena jam kerja, keinginan untuk berganti karir, serta kejelasan karir yang belum jelas.

## Bagian 4: Membangun Prediksi Perilaku Pengunduran Diri Otomatis Menggunakan _Machine Learning_
Pada tahapan ini, akan dibangun model yang dapat memprediksi indikasi penyebab resign dengan menggunakan model machine learning. Untuk pelatihan dan evaluasi model yang kuat, 287 data karyawan dibagi menjadi data training (79,79%) dan data testing (20,21%). Dengan memanfaatkan berbagai model machine learning, didapatkan insight sebagai berikut.
| Metode Machine Learning | Accuracy | Precision | Recall | F1-Score | ROC |
|---|---|---|---|---|---|
| Support Vector Machine | 0.67 | 0.0 | 0.0 | 0.0 | 0.5 |
| Gradient Boosting | 0.95 | 0.9 | 0.95 | 0.92 | 0.95 |
| Decision Tree | 0.93 | 0.86 | 0.95 | 0.9 | 0.93 |
| Random Forest | 0.91 | 1.0 | 0.74 | 0.85 | 0.87 |
| Linear Regression | 0.67 | 0.5 | 0.11 | 0.17 | 0.53 |<br>

Terlihat bahwa model Gradient Boosting menunjukkan hasil yang baik, dengan akurasi 94,83% dengan keakurasian 94,80%. Kemampuan prediksi dan keakuratannya dalam mengidentifikasi potensi pengunduran diri menjadikannya model yang direkomendasikan untuk prediksi retensi karyawan. Lalu dilakukan analisis Cross-Validation dan Hyperparameter Tuning, dimana model mengalami fine-tuning, menampilkan metrik kinerja yang cukup baik dengan:
- Rerata Precision: 0,97
- Rerata Recall: 0,96
- Rerata ROC-AUC: 0.97
<p>![image](https://github.com/user-attachments/assets/d93b3c22-ffed-40b5-b20e-f3091d04a080)<br>
Gambar disamping merupakan confusion matrix dengan pengoptimalkan hiperparameter yang menghasilkan skor AUC yang sempurna, 1.00. Pilihan hiperparameter dan skor ROC-AUC yang dihasilkan menggarisbawahi kemampuan kuat model untuk membedakan antara kasus positif dan negatif dengan diskriminasi sempurna. Hiperparameter terbaik untuk model termasuk Learning Rate: 0.01, Max Depth: 4, Min Samples Leaf: 5, Min Samples Split: 3, Number of Estimators: 50, dan Subsample: 0.8
![image](https://github.com/user-attachments/assets/bb0cfd09-6de8-41e7-8335-b9ad80fb6090)<br>
Selanjutnya, akan dilakukan analisis _feature importance_, dimana terlihat bahwa pentingnya fitur `AlasanResign` menunjukkan bahwa alasan khusus yang diberikan karyawan untuk pengunduran diri mereka memberikan peran penting dalam _feature importance_ ini. Selain itu, pentingnya fitur `AsalKota_JakartaSelatan` menyiratkan bahwa letak geografis asal-usul karyawan merupakan faktor lainnya yang patut menjadi perhatian.
![image](https://github.com/user-attachments/assets/853ddd7f-3cf4-4764-9209-8922d8cc21eb)<br>
Lalu, setelah dilakukannya analisis kurva ROC (_Receiver Operating Curve_), terlihat bahwa Kurva ROC untuk model mencapai area luar biasa di bawah kurva (AUC) 0,99, yang berarti model memiliki kemampuan tinggi untuk membedakan antara karyawan yang kemungkinan akan mengundurkan diri dan mereka yang kemungkinan akan tinggal. Nilai AUC yang tinggi ini merupakan tanda yang menjanjikan bahwa model ini efektif dalam mengidentifikasi potensi pengunduran diri, yang dapat sangat berharga untuk strategi retensi karyawan.

## Bagian 5: Menyajikan Hasil _Machine Learning_ kepada Pengguna Bisnis
Selanjutnya, dibawah ini ditunjukkan plot SHAP Values dengan menggunakan Gradient Boosting (kiri) dan Neural Network (kanan)
![image](https://github.com/user-attachments/assets/8051b0a3-8840-4540-8e7c-fad874684719)<br>
Baik model Gradient Boosting dan Neural Network memperlihatkan pentingnya faktor-faktor seperti alasan resign dan usia karyawan sebagai penentu retensi karyawan. Alasan pengunduran diri harus dipantau dengan ketat, dan masa jabatan karyawan perlu dipupuk dan dihargai. Namun, Neural Network menekankan pentingnya lama menjabat dan hari hiring, menunjukkan bahwa memelihara pertumbuhan karyawan dan mengoptimalkan proses onboarding sangat penting untuk retensi. Menggabungkan wawasan dari kedua model dapat menyebabkan pendekatan yang lebih komprehensif untuk retensi karyawan. Dengan mengatasi fitur-fitur utama ini, perusahaan dapat secara proaktif mengurangi omset, meningkatkan kepuasan karyawan, dan akhirnya meningkatkan kinerja bisnis mereka.
