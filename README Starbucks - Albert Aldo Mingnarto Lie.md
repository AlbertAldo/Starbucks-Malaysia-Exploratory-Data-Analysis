# EDA (Exploratory Data Analysis) - Starbucks Customer Survey

 **Exploratory Data Analysis** pada Dataset Starbucks Customer Survey di Malaysia pada Tahun 2019 untuk mendapatkan Informasi / Insight yang dibutuhkan berdasarkan data survey customer yang diperoleh dan memberikan Rekomendasi yang dapat diberikan melalui Insight yang didapatkan.

EDA (Exploratory Data Analysis) - Starbucks Customer Survey ini menggunakan dataset dari yg diperoleh dari :
https://www.kaggle.com/mahirahmzh/starbucks-customer-retention-malaysia-survey

Exploratory Data Analysis ini dibagi dalam 4 tahap yaitu :
1. Mempelajari Dataset
2. Define Problem and Goals
3. Mengambil Insight dari Dataset
4. Memberikan Rekomendasi

## 1. Mempelajari Dataset
Mempelajari Dataset meliputi :
```
- Pengecekan Tipe data
  (object, int64)
- Pengecekan Missing Value
  Kami menemukan 1 data kosong pada kolom Method dan Promo Method, sehingga kami mengambil keputusan dengan mengganti data kosong tersebut menjadi nilai 'never'.
- Pengecekan Outliers
  • Kami tidak menemukan outliers pada data numerik Price Rate, Promo Rate.
  • Kami menemukan outliers pada data numerik Compared Rate, Ambiance Rate, Wifi Rate, Service Rate, Choose Rate yaitu Nilai Rate "1".
- Pengecekan Kolom yg bertipe Tanggal
  Kami menemukan kolom yang bertipe tanggal yaitu terdapat pada kolom Timestamp.
```

Dalam Dataset Starbucks Customer Survey ini terdapat beberapa variabel, yaitu :
```
Variabel yang digunakan untuk membantu dalam pelaksanaan analisis
- ageframe = kolom yang berisi umur dari customers

- bayaran = perbandingan gaji pada saat shift normal dengan saat shift1 dihilangkan

- loyalty = jumlah customer yang loyal terhadap starbucks

- members = jumlah customer yang terdaftar di membership

- methodpurchasefix = berisi data metode pembelian yang dilakukan customers di starbucks

- persentase = persen penghematan setelah shift1 ditiadakan

- pesenan = jumlah pesanan yang dibeli oleh customers selama 5 hari

- promotryhard = jumlah media promo yang diketahui oleh customers

- rating = berisi nilai rata-rata rating yang diberikan customers

- shift1 = shift jam buka starbucks 00.00 - 05.59
- shift2 = shift jam buka starbucks 06.00 - 11.59
- shift3 = shift jam buka starbucks 12.00 - 17.59
- shift4 = shift jam buka starbucks 18.00 - 23.59 

- spendpurchase = kolom yang berisi jumlah spend purchase yang dilakukan oleh customers

- timedf = waktu transaksi yang dilakukan oleh customer

- timespend = berisi data waktu kunjungan customers saat berada di starbucks

- visitor = jumlah kehadiran customer berdasarkan rentang waktu tertentu

- waktu1 = jumlah customer yang datang saat shift1
- waktu2 = jumlah customer yang datang saat shift2
- waktu3 = jumlah customer yang datang saat shift3
- waktu4 = jumlah customer yang datang saat shift4

- yangdateng = jumlah customer yang datang berdasarkan jenis pekerjannya
```

## 2. Define Problem and Goals
Setelah mempelajari Dataset, kami menentukan beberapa Problem and Goals, yaitu :
```
- Bagaimana Kondisi Market dari gerai Starbucks.
- Apa yang menjadi kelebihan dan kelemahan gerai Starbucks berdasarkan data yang didapatkan.
- Menganalisa berdasarkan rating yang diberikan oleh customers.
- Bagaimana cara untuk meningkatkan Market Activity dari gerai Starbucks.
- Memberikan rekomendasi agar gerai Starbucks dapat berjalan dengan efisien dan baik.
```

## 3. Mengambil Insight dari Dataset
Setelah melakukan Define Problem and Goals kemudian dilakukan Analisis Data, dan didapatkan beberapa Insight sebagai berikut :

- Berdasarkan Spend Purchase dan Time Spend yang dilakukan oleh Customers di Starbucks : 
    ```
    - Mayoritas dari Customers melakukan Spend Purchase berada pada nilai (< RM20) dengan total transaksi 58 orang dan (RM20 - RM40) dengan total transaksi 45 orang, dari seluruh total Customers 122 orang.
    - Customers dari Starbucks di dominasi oleh orang-orang yang berumur diantara 20 - 29 tahun dan banyak diantaranya yaitu kaum perempuan.
    - Customers yang paling sedikit datang merupakan orang-orang yang berumur lebih dari 40 tahun dan berlatar belakang sebagai Housewife.
    - Customers dari kalangan yang berumur 20 tahun ke bawah sebesar 10.66%.
    - Customers yang tidak melakukan pembelian selama kunjungan di Starbucks sebesar 9.84%.
    - Mayoritas dari Customers berdasarkan Waktu Kunjungan yang dilakukan berada pada (< 30 Menit) dengan total 73 orang dan (Antara 30 menit - 1 Jam) dengan total 34 orang, dari seluruh total Customers 122 orang.
    - Tidak banyak Customers yang melakukan Waktu kunjungan di atas 2 jam.
    ```

- Berdasarkan Seberapa sering Customers datang ke Starbucks (Tabel visitor) : 
    ```
    - Total Customers yang datang 'Rarely' sebanyak 76 orang dari total 122 orang.
    - Total Customers yang datang 'Monthly' sebanyak 26 orang dari total 122 orang.
    - Total Customers yang datang 'Weekly' sebanyak 9 orang dari total 122 orang.
    - Total Customers yang datang 'Daily' sebanyak 2 orang dari total 122 orang.
    - Total Customers yang tidak pernah datang/pertama kali datang sebanyak 9 orang dari total 122 orang.
    ```

- Berdasarkan Media Promosi yang diketahui oleh Customers :
    ```
    Media Promosi
    - Social Media : 89
    - Friends and Word of Mouth : 49
    - Starbucks Website/Apps : 35
    - Display : 21
    - Email : 17
    - Billboards : 11
    - Dealsite : 7
    - Application Offer : 1
    ```

- Berdasarkan Loyalty & Membership Customers :
    ```
    - Customers yang merasa puas dan akan kembali lagi ke Starbucks sebesar 77.05%.
    - Customers yang memiliki membership sebesar 49.18% dan yang tidak memiliki membership sebesar 50.82%.
    ```

- Berdasarkan Jam Operasional Starbucks selama 5 hari:
    ```
    - Shift 1 (00:00 - 05:59) ada 2 transaksi.
    - Shift 2 (06:00 - 11:59) ada 15 transaksi.
    - Shift 3 (12:00 - 17:59) ada 71 transaksi.
    - Shift 4 (18:00 - 23:59) ada 34 transaksi.
    ```

- Berdasarkan Total Purchase Item selama 5 hari:
    ```
    - Coffee : 84
    - Cold Drinks : 38
    - Pastries : 16
    - Sandwiches : 8
    - Juices : 4
    - Jawschip : 1
    - Cake : 1
    ```

- Berdasarkan Rating yang diberikan oleh Customers :
    ```
    Rata-rata rating yang diberikan oleh masing-masing Customers dengan berbagai latar belakang sebagai berikut:
        - Employee :
            • Ambiance Rate : 3.9016
            • Choose Rate : 3.6393
            • Compared Rate : 3.7377
            • Price Rate : 2.8524
            • Promo Rate : 3.9836
            • Service Rate : 3.8852
            • Wifi Rate : 3.2787
        - Housewife :
            • Ambiance Rate : 4.0000
            • Choose Rate : 4.5000
            • Compared Rate : 4.0000
            • Price Rate : 3.0000
            • Promo Rate : 3.0000
            • Service Rate : 5.0000
            • Wifi Rate : 3.0000
        - Self-Employee :
            • Ambiance Rate : 3.8235
            • Choose Rate : 3.5294
            • Compared Rate : 3.7058
            • Price Rate : 3.2352
            • Promo Rate : 3.4705
            • Service Rate : 3.7647
            • Wifi Rate : 3.1176
        - Student :
            • Ambiance Rate : 3.5000
            • Choose Rate : 3.2857
            • Compared Rate : 3.5238
            • Price Rate : 2.8095
            • Promo Rate : 3.6904
            • Service Rate : 3.4761
            • Wifi Rate : 3.2857
    ```

## 4. Memberikan Rekomendasi 
Berdasarkan Insight yang didapat, berikut Rekomendasi yang kami berikan :
```
1. Spend Purchase dan Time Spend
Berdasarkan data yang diperoleh dari Spend Purchase dan Time Spend yang dilakukan oleh Customers, dapat dilihat bahwa waktu kunjungan Customers ke gerai Starbucks mayoritas masih dalam batas wajar yaitu sekitar 30 menit - 2 jam jika dibandingkan dengan pembelian yang dilakukan oleh Customers di gerai Starbucks. Sedangkan Customers yang melakukan kunjungan lebih dari 2 jam dapat dilihat sebagai minoritas Customers, sehingga mereka yang ingin melakukan meeting/mengerjakan tugas kuliah justru dapat menjadi potential Customers yaitu dengan cara memberikan promo yang menarik bagi mereka serta menjadikan Starbucks sebagai tempat yang nyaman untuk melakukan meeting/mengerjakan tugas kuliah.

Hal tersebut dapat menjadi strategi untuk menarik pelanggan yang datang 'Rarely' (Berdasarkan data Tabel visitor) menjadi 'Monthly' atau 'Weekly' dengan cara strategi pada poin no 2.

2. Strategi untuk Customers yang datangnya 'Rarely' menjadi 'Monthly' atau 'Weekly'
   - Bagi karyawan / perusahaan yang ingin melakukan meeting time di Starbucks, dapat melakukan reservasi area terlebih dahulu dengan melakukan pembelian Paket Meeting. 
   - Bagi mahasiswa yang ingin membutuhkan tempat untuk mengerjakan tugas / belajar, Starbucks dapat menjadi pilihan yang tepat dengan melakukan pembelian Paket Student.

3. Strategi untuk Promo
   - Branding dengan membuat konten Digital Marketing di Platform Social Media seperti Instagram, dll.
   - Branding dari Apps/Website Starbucks.
   - Promo Voucher/Cashback dari Apps Starbucks (StarbucksPay).

4. Membership
   - Free to apply.
   - Buy one get one free drink reward upon your first 5 Stars.
   - Free drink size upgrade on birthday month.
   - Pay with your mobile via StarbucksPay.
   - Order and pay first.
   - Every drink or pastries purchased get a loyalty points.
   - Invite your friends to join membership get a loyalty points.
   - Loyalty points can be change to a free menu.
   - Promo Advertise on Starbucks Apps for all members.

5. Shift Karyawan Starbucks
Asumsi Shift karyawan berdasarkan data 5 hari penjualan di Starbucks Malaysia.
- Shift 1 (00:00 - 05:59) : Barista Coffee and Colddrinks 1, Cashier 1
- Shift 2 (06:00 - 11:59) : Barista Coffee and Colddrinks 1, Cashier 1, Inventory Control 1
- Shift 3 (12:00 - 17:59) : Barista Coffee and Colddrinks 3, Cashier 2, Inventory Control 1
- Shift 4 (18:00 - 23:59) : Barista Coffee and Colddrinks 2, Cashier 1, Inventory Control 1
Asumsi : Barista RM4.3 per jam ; Cashier RM3.7 per jam

Berdasarkan data penjualan dan asumsi shift karyawan pada Starbucks Malaysia selama 5 hari, maka kami memberikan rekomendasi yang pada poin no 6 dan 7.

6. Rekomendasi untuk menutup Jam Operasional pada Shift 1 (00:00 - 05:59)
Kami memberikan rekomendasi agar menutup gerai pada Shift 1 Jam 00:00 - 05:59 dikarenakan jumlah transaksi yang sangat kecil pada shift 1. Berdasarkan dari data yang kami dapatkan selama 5 hari hanya terjadi 2 transaksi. Sehingga pengeluaran untuk gaji karyawan lebih tinggi dibanding pemasukkan yang didapat dari transaksi di shift 1. Selain biaya gaji, biaya listrik dan lainnya dapat dilakukan penghematan pada shift 1. Kami merekomendasi untuk jam buka gerai dari 6 pagi sampai 12 malam.

7. Rekomendasi Promo yang diberlakukan pada Jam Operasional Starbucks
   - Berdasarkan data dari shift 2 (07:00-11.59) diadakan Menu Breakfast untuk menarik pelanggan dipagi hari.
   - Shift 2 (07:00-11:59) diberikan promo untuk Ibu Rumah Tangga yang sedang menunggu anaknya sekolah di pagi hari.
   - Free Donuts untuk setiap pembelian minimum RM35 pada jam 13:00-17:00 dan jam 19:00-23:00.
   - Promo untuk mahasiswa dengan menunjukkan Student Card & Membership Card yaitu diskon 10% pada jam       15:00-18:00 ketika pulang sekolah.

8. Berdasarkan Total Purchase Item selama 5 hari
Untuk meningkatkan penjualan menu dari Starbucks kami merekomendasikan :
  - Membuat dan menawarkan kepada pelanggan seperti paket combo minuman + makanan.
  - Menambah varian produk minuman kopi dan cold drinks yang baru dan belum pernah ada di kompetitor yang lainnya.
  - Expand dengan membuat menu Sandwiches seperti Subways, Jiwa Toast.
  - Membuat varian produk minuman yang Limited Edition sesuai dengan event terdekat.
  - Menawarkan penjualan Tumblr Starbucks.

9. Berdasarkan Rating yang diberikan oleh Customers
Berdasarkan data rata-rata rating yang diberikan oleh Customers, Student dan Employee memberikan price rate di bawah 3, hal ini dikarenakan harga Starbucks yang memang relatif tinggi namun dengan memberikan fasilitas dan service yang baik, pelanggan pun merasa worth dan nyaman untuk datang ke Starbucks. Dapat dilihat berdasarkan data Ambiance Rate, Compared Rate, Service Rate, dan Wifi Rate yang diberikan oleh Customers.

10. Loyalty Customers
Kami merekomendasi untuk mempertahankan Service Rate dan Ambiance Rate yang diberikan oleh Customers yaitu dengan cara sebagai berikut: Seluruh karyawan Starbucks wajib memberikan pelayanan, servis, dan attitude yang terbaik terhadap pelanggan, kemudian suasana tempat cafe yang nyaman, bersih, dan dingin, serta kualitas produk kopi/makanan tetap dijaga, sehingga Customers tidak akan segan untuk datang kembali ke gerai Starbucks.
```


