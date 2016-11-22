<<<<<<< 6fb40c628c37a84901e8422fdfc5134ded6575be
Retrieve adalah bagaian dari manipulasi data yang digunakan untuk melihat isi data pada geospasial berupa data vektor yaitu yang berbentuk shape file yang diluncurkan oleh ESRI dengan extensil .shp. 

File yang dibutuhkan untuk melakukan manipulasi data yaitu:
1. shp ? berupa koordinat/titik.
2. dbf  ?berupa tabel/database.
3. shx ? berisi index data

Data vektor adalah data yang menampilkan pola keruangan dalam bentuk titik, garis, kurva atau poligon. Data vektor sangat baik untuk merepresentasikan fitur-fitur jaringan jalan, gedung, rel kereta dan letak koordinat. Kelemahan data ini adalah ketidakmampuannya dalam mengakomodasi perubahan fenomena yang bersifat gradual.
Cara menghitung jumlah record pada sebuah file yang berformat shp:

1.	masuk ke lokasi python terlebih dahulu 
2.	ketikan python 
3.	ketikan importshape file 
4.	ketikan a=shapefile.Reader ('shp/bts_negara.shp') 
5.	ketikan b=a.shapes() ketikan print len (b)

Kesimpulan : 
Dalam data Retrieve ini kita dapat melakukan select/view dan menghitung jumlah record. Dengan mendapatkan data shp kita juga belum tentu kita dapat melihat data tersebut namun kita juga harus menggunakan aplikasi sepert Qgis dan Python.

Saran :
Sebaiknya terus di terapkan pada mata kuliah GIS agar mahasiswa mengerti tentang manipulasi data geospsial karen pengetahuan seperti ini penting untuk kedepannya nanti.

Github : 

Plagiarisme :
=======
Retrieve adalah bagaian dari manipulasi data yang digunakan untuk melihat isi data pada geospasial berupa data vektor yaitu yang berbentuk shape file yang diluncurkan oleh ESRI dengan extensil .shp. 

File yang dibutuhkan untuk melakukan manipulasi data yaitu:
1. shp ? berupa koordinat/titik.
2. dbf  ?berupa tabel/database.
3. shx ? berisi index data 
Data vektor adalah data yang menampilkan pola keruangan dalam bentuk titik, garis, kurva atau poligon. Data vektor sangat baik untuk merepresentasikan fitur-fitur jaringan jalan, gedung, rel kereta dan letak koordinat. Kelemahan data ini adalah ketidakmampuannya dalam mengakomodasi perubahan fenomena yang bersifat gradual.
Cara menghitung jumlah record pada sebuah file yang berformat shp:
1.	masuk ke lokasi python terlebih dahulu 
2.	ketikan python 
3.	ketikan importshape file 
4.	ketikan a=shapefile.Reader ('shp/bts_negara.shp') 
5.	ketikan b=a.shapes() ketikan print len (b)
Kesimpulan : 
Dalam data Retrieve ini kita dapat melakukan select/view dan menghitung jumlah record. Dengan mendapatkan data shp kita juga belum tentu kita dapat melihat data tersebut namun kita juga harus menggunakan aplikasi sepert Qgis dan Python.
Saran :
Sebaiknya terus di terapkan pada mata kuliah GIS agar mahasiswa mengerti tentang manipulasi data geospsial karen pengetahuan seperti ini penting untuk kedepannya nanti.
Github : 
Plagiarisme :
>>>>>>> pertemuan 3
