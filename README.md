### PT. Skyshi Digital Indonesia
##### Jl. Tampomas No. 9, Trihanggo, Kec. Gamping,
##### Kab. Sleman, Daerah Istimewa Yogyakarta, Indonesia, 55291.
##### Phone : (0274) 4547428, Email : hello@skyshi.com 

# Project Management Guideline

## Daftar Isi
- [Introduction](#introduction)
- [Software Lifecycle](#software-lifecycle)
    - [Project Lifecycle 2018v1](#project-lifecycle-2018v1)
    - [Project Lifecycle 2018v2](#project-lifecycle-2018v2)
- [Longterm Lifecycle Project dan Product](#longterm-lifecycle-project-dan-product)
- [Project Management Guideline](#project-management-guideline)
    - [Pedoman Pelaksanaan Project](#pedoman-pelaksanaan-project)
      - [Tahap Requirement Gathering](#tahap-requirement-gathering)
      - [Tahap Inisiasi](#tahap-inisiasi)
      - [Tahap Development](#tahap-development)
      - [Tahap Deployment](#tahap-deployment)
    - [Pedoman Request Improvement dan Bug di Live Site](#pedoman-request-improvement-dan-bug-di-live-site)
    - [Pedoman Request Improvement di Ongoing Project](#pedoman-request-improvement-di-ongoing-project)
    - [Pedoman Melakukan Report Project](#pedoman-melakukan-report-project)
    - [Pedoman Menerima laporan bug dari client](#pedoman-menerima-laporan-bug-dari-client)
    
## Introduction
**Skyshi Procedure Documentation** yaitu standar dokumentasi untuk setiap divisi dalam mengelola pekerjaan yang akan memudahkan proses birokrasi dalam mengerjakan task yang diberikan, diharapkan dengan menggunakan dokumen ini pekerjaan antara divisi akan lebih mudah dan efisien.

## Software Lifecycle
### Project Lifecycle 2018v1	
   ![1](https://user-images.githubusercontent.com/45573867/61097706-87a7ba00-a486-11e9-8673-a9694614910e.png)

### Project Lifecycle 2018v2	
   ![2](https://user-images.githubusercontent.com/45573867/61097764-b4f46800-a486-11e9-947b-81ef6139cbb3.png)

## Longterm Lifecycle Project dan Product
   ![3](https://user-images.githubusercontent.com/45573867/61097780-c0e02a00-a486-11e9-93c2-c7872785a71f.png)

## Project Management Guideline	
### Pedoman Pelaksanaan Project	
Setiap project diwajibkan mengikuti prosedur berikut untuk memastikan bahwa kualitas aplikasi yang dideliver baik, dan sesuai dengan jadwal yang diberikan sehingga memberi kepastian bagi client, bagi developer, bagi tim marketing dan seluruh elemen lain yang terlibat.

#### Tahap Requirement Gathering	
-	Tahap requirement gathering adalah tahapan terpenting dalam proses project development. Pada requirement gathering dilakukan kesamaan persepsi antara product owner, bagian operation, bagian marketing, maupun sampai ke CS tentang bagaimana sebuah aplikasi membantu seluruh divisi dari product owner, operation, marketing hingga CS dalam menjalankan tugasnya masing - masing.
-	Aktivitas
    -	Meeting pertama dengan klien berupa video call atau meeting fisik
    -	Meeting kedua, setelah draft business process selesai dibuat
    -	Bagian marketing membuat penawaran resmi ke klien
    -	Bagian finance mengirimkan invoice penagihan mulai project
-	Pada tahap ini, role yang perlu terlibat adalah:
    -	System Analyst
    -	Product Owner (Client)
    -	Marketing
    -	Finance
    -	Dan divisi lain jika diperlukan seperti Marketing, Operation, CS, dll.
-	Dokumen yang dihasilkan adalah :
    -	Business Process : berisi flow, aktivitas, role berupa dokumen word atau spreadsheet (DILARANG MENGGUNAKAN KATA OVERVIEW, TASK nya harus DETAIL dan EKSPLISIT)
    -	Resource dan timeline : berisi estimasi jumlah resource yang dibutuhkan
    -	UX Flow : berisi gambaran business process secara UX flow, berdasarkan pengalaman di Skyshi, business process dalam bentuk word atau spreadsheet sulit dipahami oleh developer maupun desainer, karena itu dibutuhkan UX flow

#### Tahap Inisiasi	
-	Tahap inisiasi berguna untuk membangun kesamaan persepsi antar tim developer mulai dari backend, frontend, desainer, QA, system analyst. Tahap inisiasi ini berguna agar developer tidak bolak balik mengerjakan perubahan - perubahan seperti bug, tweaking ataupun improvement pada halaman yang sama.
-	Timeline
  -	Terdapat 2  metode pendekatan dalam penentuan timeline yang dapat digunakan dalam pengerjaan proyek di skyshi, yaitu:
    -	Waterfall (entirety) selruh tim akan mengerjakan seluruh aktifitas project dalam satu kali framework lifecycle.
    -	Sprint (iterative and incremental) Pengerjaan proyek akan dibagi mejadi beberapa bagian fase sesuai dengan prioritas kebutuhan, dan pada tiap phase nya framework lifecycle akan dilakukan kembali.
  -	Pada prosesnya penentuan timeline dimulai sebelum pengerjaan project inisiasi dimulai. System analyst dan project manager harus bisa menyusun sebuah timeline dengan pertimbangan antara lain:
    -	Kebutuhan/permintaan khusus klien
    -	Kemampuan dan jumlah resource tim
    -	Tingkat resiko sebuah proyek
    -	Ruang lingkup proyek
  -	Pertimbangan diatas sangat penting untuk dianalisa sebelum menentukan timeline. 
-	Pada tahap ini, role yang perlu terlibat adalah:
-	System Analyst
    -	System analyst memberitahukan ke Project manager bahwa sebuah project sudah siap distart. Project manager mulai mengirimkan notifikasi ke setiap tim backend, frontend, designer, QA. PM bertanggung jawab kapan mulai menjadwalkan kapan meeting pertama.
    -	Meeting pertama dengan tim developer backend, frontend, desainer, QA. Dalam meeting tersebut akan dijelaskan business process di aplikasi ini, role apa yang terlibat, database apa yang akan dipakai, target resolusi web, target resolusi untuk mobile.
-	Project Manager
    -	Project manager melakukan breakdown business process ke dokumen mapping
    -	Project manager mengumpulkan semua link dokumen ke dalam “Document link” di Zoho Documents.
    -	Semua developer, desainer mempunyai akses ke “Document link” dan dapat melihat informasi seperti login, dan link - link ke dokumen lain
    -	Presentasi meeting bersama klien, untuk menjelaskan business process dan desain yang digunakan mobile dan web. 
-	Lead Developer
    -	Backend melakukan mapping antara business process dan API yang tersedia, Backend melakukan perancangan draft endpoint API berikut struktur data seperti apa, kondisi sukses dan failed, validasi dan constraint apa yang diperlukan untuk setiap endpoint.
    -	Backend melakukan perancangan draft database 
    -	Backend melakukan perancangan draft Notifikasi yang akan dikirimkan
    -	Frontend dan slicing HTML melakukan mapping pages apa saja yang dibutuhkan di sebuah business process
-	Lead Designer
    -	Desainer melakukan mapping antara business process dan desain yang tersedia
    -	Desainer melakukan perancangan component dan perancangan halaman yang dibutuhkan sesuai dengan business process. Perancangan ini akan menampilkan desain halaman ketika ada pesan error dan pesan sukses nya seperti apa, kalau halaman ada datanya seperti apa, kalau data kosong seperti apa.
    -	Desainer menghasilkan wireframe dalam bentuk zeplin, yang dilengkapi dengan nama page yang sesuai
-	Quality Assurance
    -	QA membuat dokumen mapping UAT dan business process, pesan error, pesan sukses apa, ada data, dan data kosong seperti apa, serta validasi - validasi yang perlu dilakukan seperti apa.
-	Dokumen yang dihasilkan adalah
    -	Dokumen project task breakdown, Contoh : https://docs.google.com/spreadsheets/d/13aXxr-tHMXSAutDF4a_u5_trWefjwARpnFdWUCoRQR4/edit?usp=sharing
    -	Dokumen Business process mapping, Contoh: https://docs.google.com/spreadsheets/d/1xIldaDAwJAVm84DMrGIrdqmWEUkT3lh2q6eYckBE0Dw/edit#gid=25854119
    -	Dokumen UAT, Contoh: https://docs.zoho.com/sheet/open/b0w7974717472c76c45429d801d47314029eb/sheets/Sheet1/ranges/A1:R103
    -	Dokumen design mapping component dan screen
    -	Dokumen design user flow, Contoh: https://drive.google.com/file/d/10UTATa57dcHaSk5evv6vTXmNLIHWUWJC/view?usp=sharing
    -	Dokumen draft Wireframe, dengan nama page masing - masing
    -	Dokumen Draft API, Contoh:  https://maingame.docs.apiary.io
    -	Dokumen Draft struktur ERD,  Contoh dokumen: 
    -	Dokumen Draft notifikasi, Contoh : https://docs.google.com/spreadsheets/d/1FUK86gw7yJAocXOiDKcCepwh3nohEyT-0C_LSCQetvE/edit#gid=0
    -	Dokumen Draft API 3rd party
    -	Dokumen draft Arsitektur System, Contoh : https://docs.zoho.com/writer/open/ay1589624cab9879d4b00a46618754eface4e

## Tahap Development	
-	Pada tahap development inilah coding baru mulai dapat dilakukan. Setelah semua dokumentasi dilengkapi, dan semua persepsi tentang aplikasi yang dibangun sudah jelas.
-	Jadwal development antara desainer dan 
-	Arsitektur:
    -	SIT : staging di server lokal, menggunakan database lokal
-	Aktivitas
    -	Sysadmin menyediakan subdomain dan database. Sysadmin mengirimkan informasi subdomain dan informasi username dan nama database
    -	Backend dan Frontend bersama sama membuat server SIT dan database lokal. 
    -	Backend, frontend, desainer mengerjakan task sesuai dengan assignment
    -	Di pagi hari, backend, frontend, desainer, mengirimkan notifikasi task apa yang akan dikerjakan pada hari tersebut. Project manager melakukan summary task list dan mengirimkan summary tersebut ke klien.
    -	Di sore hari, backend, frontend, desainer, mengirimkan notifikasi task apa yang selesai dikerjakan pada hari tersebut, dan apa blocking yang ditemukan. Project manager melakukan summary task list dan mengirimkan summary tersebut ke klien.
    -	Backend, frontend, desainer mengirimkan komentar di setiap task yang selesai dikerjakan.
    -	Project manager mengirimkan summary daily dan summary weekly ke klien yang berisi progress report sebuah project.
    -	Jika ada sebuah flow yang sudah selesai dikerjakan oleh developer, maka Project Manager mengirimkan notifikasi ke Quality Assurance untuk melakukan pemeriksaaan.
    -	Setiap ada perubahan task, atau tambahan request dari client, maka Project Manager wajib melakukan pemeriksaan apakah sudah ada di business process ? Jika belum ada, maka harus dimapping ulang (apakah ada desainnya? Apakah ada API nya ? apakah ada UAT nya ?) Lanjut ke [Flow Request Improvement di Ongoing Project]
    -	Setiap request baru harus mempunyai task yang relevan. Developer dilarang mengerjakan request tanpa ada task yang relevan. Tanpa ada task, maka developer tidak mempunyai kewajiban untuk mengerjakan task tersebut.
    -	QA melakukan testing di tahap SIT secara terus menerus
-	Pada tahap ini, role yang perlu terlibat adalah
    -	Project Manager
    -	Desainer
    -	Developer
    -	Quality Assurance
-	Dokumen yang dihasilkan adalah
    -	Reporting Harian
    -	Reporting Weekly
    -	UAT dokumen automated
    -	Git repository

#### Tahap Deployment	
-	Ketika sebuah aplikasi telah dinyatakan lolos testing, dan sudah memenuhi aspek QA dari internal maupun dari sisi klien, maka dilanjutkan ke proses deployment ke live server maupun ke play store/app store.
-	Arsitektur:
    -	UAT : backend dengan latest code, database replika live terbaru
    -	Production : backend live, database live
-	Aktivitas
    -	Backend dan Frontend bersama sama membuat dokumen deployment server UAT dan Production
    -	Devops melakukan persiapan server, instalasi, konfigurasi sesuai dengan dokumen deployment server yang disediakan backend UAT dan Production
    -	Setelah aplikasi berhasil diinstall di server, maka devops wajib menjalankan prosedur checklist server :
    -	Uji coba reboot server, dan pastikan aplikasi tetap berjalan secara otomatis
    -	Pastikan semua API dan http access menggunakan https
    -	Jika menggunakan letsencrypt pastikan cron sudah terpasang untuk automatic renewal, dan nginx juga automated reload
    -	Pastikan semua log backend INFO maupun ERROR tersimpan di logentries, atau loggly yang dapat diakses di cloud
    -	Pastikan monitoring terpasang, jika server down maka otomatis devops mendapat notifikasi
-	QA menjalankan proses QA secara otomatis yang telah disimpan pada tahap development
-	User melakukan testing di tahap UAT, bukan QA karena QA melakukan testing di level SIT. Semua laporan error log dikumpulkan dulu dari user, perbaikan dilakukan esok hari. Dari laporan setiap user ini kemudian dikumpulkan lagi oleh PM atau QA, kemudian di group berdasarkan laporan yang mirip. Kemudian hasil dari group laporan ini disampaikan ke developer.
-	Pada tahap ini Role yang terlibat adalah
    -	Devops
    -	Developer
    -	QA
    -	Project Manager
-	Dokumen yang dihasilkan adalah
    -	Dokumen Deployment Server
    -	Dokumen Deployment Mobile
    -	Dokumen Serah Terima Aplikasi
    -	Dokumen Migration Plan (Jika business process berbeda, maka Backend atau Frontend wajib membuat dokumen planning migrasi dari yang lama ke yang baru. Wajib ada estimasi down time)

### Pedoman Request Improvement dan Bug di Live Site	
1.	Project manager menerima laporan request bug dan improvement dari client
2.	Project manager melakukan verifikasi error tersebut dan melakukan pengujian apakah error tersebut dapat diduplikasi
3.	Project manager melakukan review pada business process, 
    -	Jika laporan tersebut ada di business process namun tidak berjalan sesuai maka disebut bug
    -	Jika laporan tersebut tidak ada di business process, maka dapat disebut sebagai improvement
4.	Jika laporan tersebut adalah bug, maka project manager dapat menentukan tingkat urgency dari laporan tersebut.
    -	Project manager melakukan kategorisasi bug, apakah hanya mempengaruhi tampilan atau juga mempunyai impact langsung ke transaksi
    -	Project Manager dapat menggunakan Google Analytics untuk menentukan impact dari sebuah halaman yang mengalami gangguan.
    Contoh : 
    -	Tampilan
    -	Jika bug tersebut impact di tampilan 50-100% maka dapat dijadwalkan untuk dikerjakan dalam 5 hari kerja
    -	Jika bug tersebut impact di tampilan 0-50% maka dapat dijadwalan untuk diperbaiki pada next deployment
    -	Transaksi
    -	Jika bug tersebut mempunyai impact pada transaksi 70 - 100% dari user maka bug tersebut wajib difix pada hari yang sama. Dan developer yang terkait harus segera dinotifikasi.
    -	Jika bug tersebut mempunyai impact pada transaksi 50 - 70% dari user maka bug tersebut wajib difix pada keesokan harinya. Dan developer yang terkait harus segera dinotifikasi.
    -	Jika bug tersebut mempunyai impact pada transaksi 20 - 50% dari user maka bug tersebut dijadwalkan untuk dikerjakan dalam 5 hari kerja.
    -	Jika bug tersebut mempunyai impact pada transaksi kurang dari 0 - 20% dari user maka bug tersebut dapat dijadwalkan masuk pada development saat ini, dan akan diperbaiki pada next deployment.
5.	Jika laporan tersebut adalah improvement, tidak masuk di business process, maka dapat dikerjakan pada next phase, bukan di phase saat ini.
    -	Project manager memasukkan request tersebut pada business process dokumen, dan menambahkan version baru
6.	Backend dan Frontend melakukan update di SIT, QA lalu melakukan pengujian dengan SIT. User melakukan testing di tahap UAT, bukan QA karena QA melakukan testing di level SIT. Semua laporan error log dikumpulkan dulu dari user, perbaikan dilakukan esok hari. Dari laporan setiap user ini kemudian dikumpulkan lagi oleh PM atau QA, kemudian di group berdasarkan laporan yang mirip. Kemudian hasil dari group laporan ini disampaikan ke developer.
7.	Jika business process berbeda, maka Backend atau Frontend wajib membuat dokumen planning migrasi dari yang lama ke yang baru. 
8.	Jika SIT lolos, maka devops dapat melakukan update ke Live.

### Pedoman Request Improvement di Ongoing Project
1.	Setiap hari project manager mengirimkan daily report ke client
2.	Setiap pagi dan sore hari project manager melakukan meeting antar internal developer team
3.	Project manager menerima input dari internal developer team dan daily report ke client, jika ada feedback request baru yang perlu ditambahkan, maka cek kembali ke business process

### Pedoman Melakukan Report Project
#### Report dilakukan oleh Project Manajemen setiap hari dan mingguan untuk memudahkan pihak manajemen dalam mengecek progress report 
#### Pihak yang terlibat pada tahapan ini yaitu : PM, Client dan Engineer
#### Pedoman Melakukan Report Project 
- Setiap engineer melakukan breakdown task di awal project atau di awal sprint, breakdown task ini berisi estimasi lama kerja untuk setiap task
- Di akhir hari, engineer melakukan update ke task dengan rincian : isi komentar secara singkat disertai dengan screenshot  dan update status serta durasi lama kerja jika sudah selesai. 
- Keesokan harinya, PM melakukan summary task yang sudah dikerjakan di hari sebelumnya dan melaporkan prosentase project yang sudah diselesaikan di channel.
- Laporan disimpan di Google Spreadsheet
- Laporan harian dapat diteruskan ke klien (jika diperlukan)
- Laporan mingguan wajib dikirimkan setiap minggu dan PM wajib mengirimkan summary task yang sudah dikerjakan pada minggu tersebut.

### Pedoman Menerima laporan bug dari client
- Setelah PM menerima laporan maka balas chat tersebut dengan format : "akan kami duplikasi tersebut"
- PM meneruskan laporan ke QA dan mention ke tim QA melalui chat
- QA melakukan duplikasi issue hasil laporan client
- Jika issue berhasil diduplikasi maka QA melaporkan ke PM serta memberikan informasi ke grup chat bahwa issue sudah berhasil diduplikasi.
- Jika issue tidak dapat diduplikasi, maka QA menanyakan lebih lanjut ke grup chat mengenai bagaimana duplikasinya.
- Setelah berhasil dilakukan duplikasi, maka lanjutkan apakah bug tersebut sudah didefine di Business Process dan UAT
- Hasil pengecekan ada atau tidaknya di Business Process dilanjutkan oleh QA melaporkan ke PM dan PM melaporkan ke client mengenai bug tersebut sudah/belum didefine di Business Process.
- Jika tidak ada di Business Process, maka laporkan ke System Analyst agar dibuat estimasi dan jadwal sprint selanjutnya.
- Jika ada di Business Process, maka laporkan ke tech lead agar segera update jadwal dan dilakukan pengecekan prioritasnya.
- PM wajib menyediakan data impact user serta prosentase user yang mendapatkan impact di bug yang dapat didapatkan dari firebase atau GA.
- Prioritas diatur berdasarkan berdasrkan impact tersebut.
- Informasi mengenai impact dijelaskan kepada client agar dapat diatur priority nya kapan akan diupdate.

