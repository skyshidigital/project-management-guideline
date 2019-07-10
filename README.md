Project Management Guideline
===========================

### Daftar Isi

- [Pedoman Melakukan Report Project](#pedoman-melakukan-report-project)
- [Pedoman Menerima laporan bug dari client](#pedoman-menerima-laporan-bug-dari-client)

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
