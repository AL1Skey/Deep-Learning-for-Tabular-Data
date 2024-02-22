[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/MFOlW9ej)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=13482499&assignment_repo_type=AssignmentRepo)
# Live Code 7 - Set 1

---

## Assignment Objectives

*Live Code 7* ini dibuat guna mengevaluasi konsep Artificial Neural Network pada pembelajaran Phase 2 sebagai berikut:

- Mampu memahami konsep Artificial Neural Network.
- Mampu mempersiapkan data untuk digunakan dalam model Artificial Neural Network.
- Mampu mengimplementasikan Artificial Neural Network dengan data yang diberikan.
- Mampu menganalisis dan menjelaskan layer yang dibuat.

---

## Dataset Description

Dataset : `hotel.csv`

| Column | Description |
| --- | --- |
| Booking_ID | Unique identifier of each booking |
| no_of_adults | Number of adults |
| no_of_children | Number of children |
| no_of_weekend_nights | Number of weekend nights (Saturday or Sunday) the guest stayed or booked to stay at the hotel |
| no_of_week_nights | Number of weekday nights (Monday to Friday) the guest stayed or booked to stay at the hotel |
| type_of_meal_plan | Type of meal plan booked by the customer <br><br> `Not Selected` – No meal plan selected <br> `Meal Plan 1` – Breakfast <br> `Meal Plan 2` – Half board (breakfast and one other meal) <br> `Meal Plan 3` – Full board (breakfast, lunch, and dinner) |
| required_car_parking_space | Does the customer require a car parking space? (`0` - No, `1`- Yes) |
| room_type_reserved | Type of room reserved by the customer |
| lead_time | Number of days between the date of booking and the arrival date |
| arrival_year | Year of arrival date |
| arrival_month | Month of arrival date |
| arrival_date | Date of the month |
| market_segment_type | Market segment designation |
| repeated_guest | Is the customer a repeated guest? (`0` - No, `1`- Yes) |
| no_of_previous_cancellations | Number of previous bookings that were canceled by the customer prior to the current booking |
| no_of_previous_bookings_not_canceled | Number of previous bookings not canceled by the customer prior to the current booking |
| avg_price_per_room | Average price per day of the reservation; prices of the rooms are dynamic. (in Euros) |
| no_of_special_requests | Total number of special requests made by the customer (e.g. high floor, view from the room, etc) |
| booking_status | Flag indicating if the booking was canceled or not |

---

## Problems 

Sebuah perusahaan yang bergerak dalam bidang perhotelan ingin meminimalisir jumlah pemesanan kamar hotel yang dibatalkan oleh customer. Bantulah perusahaan tersebut untuk memprediksi customer yang akan membatalkan pesanan dari dataset yang diberikan.
Dataset terlampir pada repository.

---

## Assignment Instructions

*Live Code 7* dikerjakan dalam format *notebook* dengan beberapa *kriteria wajib* di bawah ini:

1. Deep Learning framework yang digunakan adalah *TensorFlow*.

2. Ada penggunaan library visualisasi, seperti *matplotlib*, *seaborn*, atau yang lain.

3. Isi *notebook* harus mengikuti *outline* di bawah ini:
   1. Perkenalan
      > Bab pengenalan harus diisi dengan identitas, gambaran besar dataset yang digunakan, dan *objective* yang ingin dicapai.
   
   2. Import Libraries
      > *Cell* pertama pada *notebook* **harus berisi dan hanya berisi** semua *library* yang digunakan dalam *project*.
   
   3. Data Loading
      > Bagian ini berisi proses penyiapan data sebelum dilakukan eksplorasi data lebih lanjut. Proses Data Loading dapat berupa memberi nama baru untuk setiap kolom, mengecek ukuran dataset, dll.
   
   4. Exploratory Data Analysis (EDA)
      > Bagian ini berisi explorasi data pada dataset diatas dengan menggunakan query, grouping, visualisasi sederhana, dan lain sebagainya.

   5. Feature Engineering
      > Bagian ini berisi proses penyiapan data untuk proses pelatihan model, seperti pembagian data menjadi train-val-test, transformasi data (normalisasi, encoding, dll.), dan proses-proses lain yang dibutuhkan.   
   
   6. ANN Training - Sequential API
      
      vi.1. Model Definition
      > Bagian ini berisi cell untuk mendefinisikan model. Jelaskan alasan menggunakan suatu algoritma/model, hyperparameter yang dipakai, jenis penggunaan metrics yang dipakai, dan hal lain yang terkait dengan model.

      vi.2. Model Training
      > Cell pada bagian ini hanya berisi code untuk melatih model dan output yang dihasilkan. Lakukan beberapa kali proses training dengan hyperparameter yang berbeda untuk melihat hasil yang didapatkan. Analisis dan narasikan hasil ini pada bagian Model Evaluation.
   
      vi.3. Model Evaluation
      > Pada bagian ini, dilakukan evaluasi model yang harus menunjukkan bagaimana performa model berdasarkan metrics yang dipilih. Hal ini harus dibuktikan dengan visualisasi tren performa dan/atau tingkat kesalahan model. **Lakukan analisis secara detail terkait dengan hasil pada model dan tuliskan hasil analisisnya**.

   7. ANN Training - Functional API
      
      vii.1. Model Definition
      > Bagian ini berisi cell untuk mendefinisikan model. Jelaskan alasan menggunakan suatu algoritma/model, hyperparameter yang dipakai, jenis penggunaan metrics yang dipakai, dan hal lain yang terkait dengan model.

      vii.2. Model Training
      > Cell pada bagian ini hanya berisi code untuk melatih model dan output yang dihasilkan. Lakukan beberapa kali proses training dengan hyperparameter yang berbeda untuk melihat hasil yang didapatkan. Analisis dan narasikan hasil ini pada bagian Model Evaluation.
   
      vii.3. Model Evaluation
      > Pada bagian ini, dilakukan evaluasi model yang harus menunjukkan bagaimana performa model berdasarkan metrics yang dipilih. Hal ini harus dibuktikan dengan visualisasi tren performa dan/atau tingkat kesalahan model. **Lakukan analisis secara detail terkait dengan hasil pada model dan tuliskan hasil analisisnya**.
   
   8. Model Saving
      > Pada bagian ini, dilakukan proses penyimpanan model dan file-file lain yang terkait dengan hasil proses pembuatan model. Pilihlah 1 arsitektur ANN yang terbaik berdasarkan hasil evaluasi sebelumnya. **Nyatakan secara jelas arsitektur mana yang akan dipakai sebagai model terbaik (Sequential API atau Functional API).**
   
   9. Model Inference
      > Model yang sudah dilatih akan dicoba pada data yang bukan termasuk ke dalam train-set, val-set, ataupun test-set. Data ini harus dalam format yang asli, bukan data yang sudah di-scaled. **Model Inference harus berada pada notebook yang berbeda dari notebook yang dipakai untuk pembuatan model.**
   
   10. Pengambilan Kesimpulan
       > Pada bagian terakhir ini, **harus berisi** kesimpulan yang mencerminkan hasil yang didapat dengan *objective* yang sudah ditulis di bagian pengenalan.

4. *Notebook* harus diupload dalam akun GitHub Classroom masing-masing siswa untuk selanjutnya dinilai.

---

## Assignment Submission

- Simpan assignment pada sesi ini dengan nama `P2LC7_Set_1_<nama-student>.ipynb`, misal `P2LC7_Set_1_raka_ardhi.ipynb`.

- Anda tidak perlu mengupload model ke GitHub karena dikhawatirkan ukurannya melebihi batas ukuran maksimum file yang diizinkan oleh GitHub.

- Push Assigment yang telah Anda buat ke akun Github Classroom Anda masing-masing.

- Contoh bentuk isi repository.
    ```
    ├── P2LC7_Set_1_raka_ardhi.ipynb
    ├── P2LC7_Set_1_raka_ardhi_inference.ipynb
    ├── hotel.csv
    └── README.md
    ```

---

## Assignment Rubrics

### Code Review

| Criteria|Meet Expectations|Points|
| --- | --- | --- |
| Feature Engineering | Mampu melakukan preprocessing dataset sebelum melakukan proses modeling (split data, normalisasi, encoding, dll) | 35 pts |
| ANN Training - Sequential API | Membuat model Artifical Neural Network dengan menggunakan Sequential API | 13 pts |
| ANN Training - Functional API | Membuat model Artifical Neural Network dengan menggunakan Functional API | 13 pts |
| Model Inference | Mencoba model yang telah dibuat dengan data baru | 10 pts |
| Runs Perfectly | Kode berjalan tanpa ada error. Seluruh kode berfungsi dan dibuat dengan benar | 10 pts |

```
Catatan mengenai ANN Training - Sequential API : 

1. Buatlah model ANN dengan Sequential API yang terdiri dari minimal 5 buah Hidden Layer.
2. Narasikan mengenai layer yang Anda buat beserta hyperparameter yang Anda tulis.
3. Sebaiknya lakukan training dengan lebih dari 20 epochs agar dapat terlihat performa model dengan lebih jelas.
4. Anda tidak diperkenankan menggunakan transfer learning.
5. Anda dipersilakan menggunakan TensorFlow Callback.

Catatan mengenai ANN Training - Functional API :

1. Buatlah model ANN dengan Functional API seperti pada URL berikut ini : https://i.ibb.co/z6Wd3xq/P2-LC7-ANN-Functional-API.png
2. Narasikan mengenai layer yang Anda buat beserta hyperparameter yang Anda tulis.
3. Sebaiknya lakukan training dengan lebih dari 20 epochs agar dapat terlihat performa model dengan lebih jelas.
4. Anda tidak diperkenankan menggunakan transfer learning.
5. Anda dipersilakan menggunakan TensorFlow Callback.

```

### Readability

| Criteria | Meet Expectations | Points|
| --- | --- | --- |
| Tertata Dengan Baik | Semua baris kode terdokumentasi dengan baik dengan menggunakan Markdown untuk penjelasan kode. | 15 pts |

```
Kriteria tertata dengan baik diantaranya adalah : 

1. Terdapat section Perkenalan yang jelas
2. Tidak menyalin markdown dari tugas lain.
3. Import library rapih (terdapat dalam 1 cell dan tidak ada unused libs).
4. Pemakaian fungsi markdown yang optimal (Heading, text formating, dll). 
5. Terdapat komentar pada setiap baris kode.
6. Adanya pemisah yang jelas antar section, dll.
7. Tidak adanya typo.
```

### Analysis

| Criteria | Meet Expectations | Points|
| --- |--- |--- |
| Model Analysis | Menganalisa informasi dari model yang telah dibuat | 35 pts |
| Overall Analysis | Menarik informasi/kesimpulan dari keseluruhan kegiatan yang dilakukan | 10 pts |

```
Contoh kriteria analisa yang baik diantaranya adalah: 

1. Terdapat penjelasan macam-macam hasil metric evaluasi dan interpretasinya terhadap kasus yang diselesaikan.
2. Dapat menjelaskan kelemahan/kekurangan dan kelebihan dari model yang dibuat.
3. Dapat memberikan statement untuk improvement selanjutnya dari model yang dibuat. 
4. Sebutkan insight yang dapat diambil setelah proses EDA, dll.
```

---

```
Total Points : 141
```

---
## Notes

* **Deadline : pukul 12:15 WIB.**

* **Keterlambatan pengumpulan tugas mengakibatkan skor LC 7 menjadi 0.**
