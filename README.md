# Final_Project_Home_Credit_Indonesia

Nama : Muhammad Farhan Darmawan

Batch : RMT 019

# Link for Deployment : https://huggingface.co/spaces/farhandraka/Home-Credit-Indonesia-Prediction

# **Project Description :**

Memprediksi customer behavior yang dimiliki oleh HOME CREDIT INDONESIA apakah sulit membayar atau tidak menggunakan machine learning (supervised learning) dengan algoritma CatBoost, Random Forest, dan XGBoost

# **Conclusion :**

## **Exploratory Data Analysis :**


Berdasarkan analisis terhadap berbagai faktor yang mempengaruhi perilaku pelanggan dalam membayar pinjaman, beberapa kesimpulan dapat diambil. Pertama, pelanggan dengan pendapatan total yang rendah, jumlah kredit yang kecil, harga barang yang terbatas, dan anuitas pinjaman yang rendah cenderung mengalami kesulitan dalam membayar pinjaman. Keluarga dengan jumlah anggota yang sedikit, usia pelanggan muda, dan status baru mendapatkan pekerjaan juga dapat menghadapi kesulitan dalam pembayaran.

Selanjutnya, jenis kontrak pinjaman (cash loans), kepemilikan real estate tanpa keinginan memiliki mobil, dan status perkawinan juga berpotensi menjadi faktor yang sulit membayar pinjaman. Tipe penghuni yang tidak didampingi (unaccompanied) dan pendidikan menengah khusus (secondary special) juga dapat mempengaruhi perilaku pelanggan dalam membayar pinjaman.

Selain itu, sumber pendapatan dari pekerjaan (working), asosiasi komersial (commercial associate), dan pensiunan (pensioner) serta kepemilikan aset rumah atau apartemen dapat berhubungan dengan kesulitan pembayaran pinjaman. Tidak memiliki telepon kerja, tetapi memiliki telepon seluler dan rumah yang mudah dihubungi melalui telepon tanpa email juga dapat menjadi indikasi kesulitan dalam pembayaran pinjaman.

Faktor lain yang dapat mempengaruhi perilaku pelanggan adalah rating wilayah tinggal, alamat permanen dan alamat kontak yang sama, tipe hunian blok apartemen, dan bahan bangunan rumah. Pelanggan yang tidak menyediakan seluruh dokumen yang diperlukan juga dapat menghadapi kesulitan dalam membayar pinjaman.

Terakhir, jenis pekerjaan seperti buruh, staf inti, pengemudi, manajer, dan staf penjualan, serta jenis organisasi atau perusahaan tertentu (business entity type 3, XNA, dan self-employed) dapat berhubungan dengan kesulitan dalam pembayaran pinjaman.

Kesimpulannya, ada banyak faktor yang dapat mempengaruhi perilaku pelanggan dalam membayar pinjaman. Faktor-faktor seperti pendapatan rendah, jumlah kredit, harga barang, anuitas pinjaman, keluarga, status pekerjaan, kepemilikan aset, jenis kontrak pinjaman, tipe penghuni, pendidikan, status perkawinan, jenis rumah, dokumen yang disediakan, jenis pekerjaan, dan jenis organisasi/perusahaan semua dapat berkontribusi terhadap kesulitan pelanggan dalam membayar pinjaman.

## **Model Analysis :**

Dari ketiga model yang telah digunakan, model CatBoost merupakan model terbaik karena memiliki nilai ROC-AUC sekitar 74% dibandingkan kedua model lainnya

Model masih *Under Fitting* karena imbalance nya data pada kolom `TARGET`

Feature Importance yang memberikan kontribusi paling tinggi yaitu `YEAR_LAST_PHONE_CHANGE`, `YEAR_EMPLOYED`, dan `AMT_REQ_CREDIT_BUREAU_YEAR`

## **Insight / Reccomendation :**

Untuk Data dikarenakan inbalance perlunya untuk memiliki dataset yang balance pada TARGET (binary classification) hal ini memberikan dampak pada model untuk memprediksi customer

Untuk meningkatkan nilai metric, dapat dilakukan feature selection, selain itu dapat melakukan pengembangan model lebih lanjut

Untuk **HOME CREDIT INDONESIA** saat customer mencoba melakukan registrasi, dapat dilakukan assessment terlebih dahulu apakah customer tersebut layak mendapatkan pinjaman atau tidak, untuk mengurangi kerugian dan meng-antisipaasi customer yang nantinya sulit untuk membayar tagihan pinjaman
