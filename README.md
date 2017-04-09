# Berlin Mitra Putra Aryadi
D4-TI-2A
Tugas Web Service 2 - XSD Schema

Penjelasan :

Jasa.xml

<?xml version="1.0" encoding="UTF-8"?>
<IndustriJasa xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="Jasa.xsd">
	<LowonganKerja>
		<post>Mirana</post>
		<judul>Re-Design Website</judul>
		<pekerjaan>Pengembangan User Interface Design</pekerjaan>
		<skill>HTML dan CSS</skill>
		<kebutuhan>5 Orang</kebutuhan>
		<pembukaan>25-01-2017</pembukaan>
		<penutupan>30-01-2017</penutupan>
		<tempo_waktu>6 Hari</tempo_waktu>
		<pendaftaran>Portofolio</pendaftaran>
		<komisi>500000</komisi>
	</LowonganKerja>
</IndustriJasa>

1. Pada dokumen XML diatas terdapat instruksi proses / Sebuah direktif khusus untuk pengolahan dokumen XML 
   <?xml version="1.0" encoding="UTF-8"?>
   yang mempunyai karakter data seperti : encoding, yang menjelaskan Semua karakter dalam dokumen XML 
   harus mengikuti pengkodean dokumen.

2. Pada dokumen XML diatas terdapat 10 elemen,seperti :
   	<post>Mirana</post>
		<judul>Re-Design Website</judul>
		<pekerjaan>Pengembangan User Interface Design</pekerjaan>
		<skill>HTML dan CSS</skill>
		<kebutuhan>5 Orang</kebutuhan>
		<pembukaan>25-01-2017</pembukaan>
		<penutupan>30-01-2017</penutupan>
		<tempo_waktu>6 Hari</tempo_waktu>
		<pendaftaran>Portofolio</pendaftaran>
		<komisi>500000</komisi>
    10 element diatas adalah sebuah isi / informasi yang ada pada file Jasa.XML
    merupakan komponen yang berfungsi memberikan informasi tambahan terhadap element yang elementnya terdapat dibawah 
    atribut tersebut.
    
3. Pada dokumen XML diatas juga sudah terintegrasi dengan XML schema, yang menjelaskan bahwa file lokasi yang dibuat pada file
   Jasa.xsd sudah bisa melakukan validasi terhadap file XML yang dialamatkan melalui generate Jasa.xsd ke Jasa1.xml apabila
   dokumen yang ada didalam Jasa1.xml 
   xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="Jasa.xsd"
   sudah di copy kedalam file Jasa.xml dan bisa melakukan validasi, berarti tidak ada file skema lokasi yang terganggu / bisa 
   disebut sudah serasi.
   
 
 Jasa.xsd :
 
 1. Tujuan pembuatan file xsd adalah kita dapat mengetahui lokasi-lokasi elemen pada sebuah elemen xml yang sebelumnya 
    sudah dibuat
 
 2. Kita dapat mengatur ketentuan type-type yang terdapat pada elemen tersebut, seperti :
    mengatur Constraint pada type string untuk memberikan sebuah pendek dan panjangnya sebuah tulisan yang ingin dibuat.
    mengatur Constraint pada type int untuk memberikan sebuah minimal dan maximal jumlah yang ingin kita tujukan.
 
 
 Jasa1.xml :
 
<?xml version="1.0" encoding="UTF-8"?>
<alamat xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="Jasa.xsd">alamat</alamat>
file tersebut terbuat / terbentuk melalui generate pada file xsd, tujuannya untuk melakukan pengintegrasian pada file xml yang
sebelumnya sudah dibuat, karena apabila namespace yang terdapat pada hasil generate file xsd dapat melakukan validasi / bisa di
validasi, berarti skema lokasi yang ada pada file xsd sudah terintegrasi terhadap xml yang sebelumnya sudah dibuat.
