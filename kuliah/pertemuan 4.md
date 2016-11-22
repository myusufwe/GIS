Retrieve data geospasial adalah merupakan suatu cara untuk melakukan select/view, data record dari file dbf dan geometri dari file shp.
Dalam pembahasan kali ini Retreive data geospasial yaitu dengan mengambil data vector ESRI/shapefile dibagi 2 terdapat DBF dan SHP. Terdapat 3 Geometri standar ESRI
1.      Point
2.      Poline
3.      Poligon
Penjelasan:

Poin = dalam peta biasanya menunjukan sebuah tempat misalnya restoran
Polygon = dalam peta biasanya menunjukan sebuah pulau
Perbedaan Polygon dan Polyline adalah titik awal dan akhir polygon selalu bertemu sedangkan tidak dengan polyline.

Operasi pada Python: 

Implementasi Retrieve Data Geospasial dalam python:

>>sf = shapefile.Reader(‘namafile.shp’)
sf adalah variable
shapefile adalah nama class
Reader adalah nama method
Perintah untuk mengambil data perkolom:

>>sf.record(n)[n]
Perintah untuk melihat isi shapefile:

>>a = sf.shape(0)
>>dir(a)
Untuk melihat type:

>> a.shapetype


Mencari negara:

>> for a in sf.records():
>>   if a[8] == “indonesia”
>>         print a
Melihat Baris:

>> Print i
>>   i = i + 1

Kesimpulan :
Jadi dalam meretrive data kita dapat melakukan select atau view dan menghitung jumlah record tentunya dengan menggunakan aplikasi sepert Qgis dan Python.
Saran :
Terus di terapkan kepasa mahasiswa agar mengerti tentang data retrive pada data geosapsial.
