Retrieve data geospasial adalah merupakan suatu cara untuk melakukan select/view, data record dari file dbf dan geometri dari file shp.

A. Cara Membuat Data Geospasial

Untuk membuat data geospasial, menggunakan library pyshp, dan untuk membuat data geospasial diperlukan file namafile.shp beserta namafile.dbf.
Adapun tahapannya sebagai berikut:

	a. Import shapefile
	b. Instanisasu writer method
    		Sf = shapefile.Writer(param)
    		Dimana param adalah pilih shapetype:
		- shapeType = 1
		- shapeType = 3
		- shapeType = 5

c. Sama seperti read, kita lakukan method dbf dan shp.

 Shapefile (shp)
 Untuk menambahkan record tergantung dengan tipe ESRI-nya.
	1. sf.point (x,y)
	2. sf.line = (parts:[[x.y],[z.w],...])
	3. sf.poly = (parts:[[x.y],z.w],...])
 	Databasefile (dbf)

 Tahapannya adalah sebagai berikut:

a. Membuat atribut terlebih dahulu kemudian menambahkan record nya.
Contoh:
sf.field('Nama Field','C','50')
Dimana C adalah Character, dan 50 adalah length. Dalam arti nama atribut, nama field dengan panjang 50 karakter.

b. Tambahkan recird dibawah ini
 sf.record('Batam')
 sf. record('Batam','Sekupang')

c. Setelah selesai maka simpan, dengan perintah
 sf.save('namafile.shp')

B. EDITING DATA GEOSPASIAL

Adapun dalam editing data geospasial hampir sama dengan langkah-langkah membuat data geospasial, yang membedakan adalah:

sf = shapefile.Writer(param)
diganti dengan

sf = shapefile.Editor(param)

dimana param adalah nama letak file.

Adapun operasi dalam editing pada shp dan dbf sama saja.
shp		dbf
sf.poly()
sf.line()
sf.point()	sf.record()

sf.delete(n), dimana n adalah baris ke-n dari tabel



Dan jika sudah selesai, simpan dengan perintah:
Sf.save(‘namafile’)

Kesimpulan :
untuk membuat data geospasial adalah WRITE sedangankan untuk mengedit adalah EDITOR.

Saran :
Untuk mengedit dan membuat data geospasial kita sebaiknya mempelajari terlebih dahulu bahasa pemrogramanya yaitu bahasa pemrograman Phython.
