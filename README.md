# Exploratory Data Analysis Segmentasi Pelanggan Supermarket
## [Capstone 2 JCDS Purwadhika]
---

# **Pengantar**
Supermarket "Fiction Mart" adalah perusahaan ritel yang tengah berusaha meningkatkan penjualan pada berbagai platform, seperti situs web, katalog, dan toko fisik, serta meningkatkan penjualan lini produknya diantaranya seperti anggur (wines), buah-buahan (fruits), daging (meat), ikan (fish), makanan manis (sweet), dan bahkan perhiasan emas (gold). Untuk mencapai tujuan ini, tim Sales & Marketing telah memulai sebuah inisiatif penting.

Mereka memutuskan untuk melihat lebih dekat pada data transaksi pelanggan yang telah menjadi anggota loyal mereka dalam rentang waktu dari pertengahan 2012 hingga pertengahan 2014. Tujuan utama dari analisis ini adalah untuk menggali wawasan tentang profil pelanggan, yang mencakup faktor-faktor seperti tingkat pendidikan (Education), status perkawinan (Marital Status), pendapatan (Income), dan jumlah anak dalam keluarga. Selain itu, tim juga akan memeriksa pola transaksi pelanggan, termasuk frekuensi transaksi, total pengeluaran transaksi, seberapa baru pelanggan tersebut berbelanja (Recency), serta adanya keluhan atau komplain (Complain) yang mereka sampaikan.

Hasil dari analisis mendalam terhadap data ini akan menjadi kunci bagi tim Sales & Marketing dalam mengidentifikasi segmen pelanggan yang memiliki potensi besar untuk meningkatkan penjualan setiap produk dan platform. Dengan wawasan yang diperoleh dari data ini, mereka akan dapat mengarahkan strategi pemasaran yang lebih terfokus dan efektif, serta memberikan pengalaman berbelanja yang lebih personal kepada pelanggan.

# Rumusan Masalah

 >1. Bagaimana pola transaksi pelanggan supermarket?<br>
 >2. Apa saja karakteristik atau profil pelanggan supermarket? apakah karakteristik pelanggan berkaitan dengan pola transaksi pelanggan?<br>
 >3. Bagaimana performansi penjualan lini produk? bagaimana karakteristik dan pola transaksi pelanggan dapat mempengaruhi penjualan dari setiap lini produk?
 >4. Bagaimana performansi platform transaksi supermarket? bagaimana karakteristik dan pola transaksi pelanggan dapat mempengaruhi frekuensi traksaksi dari setiap platform?


# Bagian- Bagian dalam EDA

1. Data Understanding
2. Data Cleaning & Preparation
3. Data Analysis


# Dataset Glossary
### Supermarket Data

| Kategori               | Kolom                            | Penjelasan                                                   |
|:------------------------|:----------------------------------|:--------------------------------------------------------------|
| Data Pribadi                 | ID                               | Identifikasi unik pelanggan                                  |
|                        | Year_Birth                       | Tahun kelahiran pelanggan                                    |
|                        | Education                        | Tingkat pendidikan pelanggan                                 |
|                        | Marital_Status                   | Status pernikahan pelanggan                                  |
|                        | Income                           | Pendapatan tahunan rumah tangga pelanggan                     |
|                        | Kidhome                          | Jumlah anak-anak dalam rumah tangga pelanggan                |
|                        | Teenhome                         | Jumlah remaja dalam rumah tangga pelanggan                   |
|                        | Dt_Customer                      | Tanggal pendaftaran keanggotaan pelanggan dengan supermarket               |
|                        | Recency                          | Jumlah hari sejak pembelian terakhir pelanggan                |
|                        | Complain                         | 1 jika pelanggan mengajukan komplain dalam 2 tahun terakhir, 0 lainnya  |
| Lini Produk               | MntWines                         | Jumlah yang dihabiskan untuk anggur dalam 2 tahun terakhir   |
|                        | MntFruits                        | Jumlah yang dihabiskan untuk buah-buahan dalam 2 tahun terakhir |
|                        | MntMeatProducts                  | Jumlah yang dihabiskan untuk produk daging dalam 2 tahun terakhir |
|                        | MntFishProducts                  | Jumlah yang dihabiskan untuk produk ikan dalam 2 tahun terakhir |
|                        | MntSweetProducts                 | Jumlah yang dihabiskan untuk produk permen dalam 2 tahun terakhir |
|                        | MntGoldProds                     | Jumlah yang dihabiskan untuk produk emas dalam 2 tahun terakhir |
| Promotion              | NumDealsPurchases                | Jumlah pembelian dengan diskon                               |
|                        | AcceptedCmp1                     | 1 jika pelanggan menerima tawaran dalam kampanye pertama, 0 lainnya |
|                        | AcceptedCmp2                     | 1 jika pelanggan menerima tawaran dalam kampanye kedua, 0 lainnya |
|                        | AcceptedCmp3                     | 1 jika pelanggan menerima tawaran dalam kampanye ketiga, 0 lainnya |
|                        | AcceptedCmp4                     | 1 jika pelanggan menerima tawaran dalam kampanye keempat, 0 lainnya |
|                        | AcceptedCmp5                     | 1 jika pelanggan menerima tawaran dalam kampanye kelima, 0 lainnya |
|                        | Response                         | 1 jika pelanggan menerima tawaran dalam kampanye terakhir, 0 lainnya |
| Platform                  | NumWebPurchases                   | Jumlah pembelian melalui situs web perusahaan                 |
|                        | NumCatalogPurchases               | Jumlah pembelian dengan menggunakan katalog                   |
|                        | NumStorePurchases                | Jumlah pembelian langsung di toko                            |
|                        | NumWebVisitsMonth                 | Jumlah kunjungan ke situs web perusahaan dalam sebulan terakhir |
