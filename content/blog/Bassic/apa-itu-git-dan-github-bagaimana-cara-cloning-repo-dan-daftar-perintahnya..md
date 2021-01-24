+++
title = "APA itu Git dan Github? Bagaimana cara cloning repo? Dan daftar perintahnya."
date = 2020-11-24T23:49:00Z
updated = 2020-11-24T23:58:46Z
tags = ["Git", "Catatan"]
blogimport = true 
[author]
	name = "MuryP"
	uri = "https://www.blogger.com/profile/14798613158789333825"
+++

{{< html >}}
{{< html >}}
<h1 style="text-align: left;">APA itu Git dan Github? Bagaimana cara cloning repo? Dan daftar perintahnya.</h1><p>Hello world!</p><p>Ini adalah sebuah catatan sekaligus informasi bagi kalian mengenai <b>github</b>. Mungkin dari kalian pernah mendengarnya. Atau bagi kalian yang belum mengetahuinya tenang saja saya akan bahas satu persatu.</p><p><br /></p><p>Daftar isi :</p><p></p><ol style="text-align: left;"><li><a href="#penjelasan">Apa itu git dan github</a></li><li><a href="#perbedaan">Perbedaan</a><br /></li><li><a href="#kesimpulan">Kesimpulan</a><br /></li><li><a href="#kelebihan">Kelebihan</a><br /></li><li><a href="#repositori">Apa itu repositori</a><br /></li><li><a href="#tutorial">Cara clone repository </a><br /></li><li><a href="#perintah">Daftar perintah git dan github</a><br /></li></ol><p></p><p><br /></p><h2 id="penjelasan"style="text-align: left;">Apa itu git dan github</h2><p><b>Git</b> adalah contoh <i>sistem kontrol versi terdistribusi (DVCS)</i> yang biasa digunakan untuk pengembangan perangkat lunak open source dan komersial. DVCS memungkinkan akses penuh ke setiap file, cabang, dan iterasi proyek, dan memungkinkan setiap pengguna mengakses riwayat lengkap dan mandiri dari semua perubahan. Tidak seperti sistem kontrol versi terpusat yang dulu populer, DVCS seperti <b>Git</b> tidak memerlukan <i>koneksi</i> konstan ke repositori pusat. Pengembang dapat bekerja di mana saja dan berkolaborasi secara asinkron dari zona waktu mana pun.</p><p><br /></p><p>Tanpa kontrol versi, anggota tim tunduk pada tugas yang berlebihan, jadwal yang lebih lambat, dan banyak salinan dari satu proyek. Untuk menghilangkan pekerjaan yang tidak perlu, Git dan VCS lainnya memberikan setiap kontributor pandangan yang seragam dan konsisten dari sebuah proyek, menampilkan pekerjaan yang sedang berlangsung. Melihat riwayat perubahan yang transparan, siapa yang membuatnya, dan bagaimana mereka berkontribusi pada pengembangan proyek membantu anggota tim tetap selaras saat bekerja secara mandiri.</p><p>Source : https://guides.github.com/introduction/git-wikipedia</p><p><br /></p><h2 style="text-align: left;">Apa itu Github</h2><p>Sedangkan <b>GitHub</b> adalah layanan <i>host</i> web bersama untuk proyek pengembangan perangkat lunak yang menggunakan sistem kendali versi <b>Git</b> dan layanan <i>hosting</i> internet. Hal ini banyak digunakan untuk kode komputer. Ini memberikan kontrol akses dan beberapa<i> fitur kolaborasi</i> seperti pelacakan bug, permintaan fitur, manajemen tugas, dan wiki untuk setiap proyek.</p><p>Sumber : wikipedia</p><p><br /></p><h2 style="text-align: left;" id="perbedaan">Perbedaan</h2><p><b>Git</b> adalah <i>alat</i> sedangkan <b>github</b> adalah <i>hosting</i>. Dimana kedua sl tersebut sangat mempermudah para proggramer bekerja. Baik secara <i>team</i> maupun <i>individu</i>. Dimana kita bisa saling membagikan projek kita satu sama lain.&nbsp;</p><p><br /></p><h2 id="kesimpulan"style="text-align: left;">Kesimpulan mengenai git dan github</h2><p><b>Git</b> dan <b>github</b> merupakan alat dan hosting untuk <i>memudahkan pembuatan kode</i>. Sehingga tak ada file yang menumpuk seperti file dokumen anak kuliahan yang direvisi mulu. Selain itu juga kedua hal tersebut mempercepat pembuatan kode mulai dari komunikasi sampai jika ada kesalahan kode, kita tinggal pindah komit saja. Dan yang paling bagusnya kita bisa membuat percobaan mengenai kode kita tanpa mempengaruhi kode utama dengan branch.</p><p><br /></p><p><b>Git</b> memungkinkan pengembang melihat seluruh garis waktu <i>perubahan, keputusan, </i>dan <i>perkembangan proyek</i> apa pun di satu tempat. Dari saat mereka mengakses riwayat proyek, pengembang memiliki semua konteks yang mereka butuhkan untuk memahaminya dan mulai berkontribusi.</p><p><br /></p><h2  id="kelebihan" style="text-align: left;">Kelebihan</h2><p><br /></p><p>Pengembang bekerja di setiap zona waktu. Dengan <b>DVCS</b> seperti <b>Git</b>, kolaborasi dapat terjadi kapan saja dengan tetap menjaga integritas kode sumber. Menggunakan cabang, pengembang dapat dengan aman mengusulkan perubahan pada kode produksi.</p><p><br /></p><p><b>Bisnis</b> yang menggunakan <b>Git</b> dapat <i>meruntuhkan</i> <i>hambatan</i> <i>komunikasi</i> antar tim dan membuat mereka tetap fokus untuk melakukan pekerjaan terbaiknya. Selain itu, Git memungkinkan untuk menyelaraskan para ahli di seluruh bisnis untuk berkolaborasi dalam proyek-proyek besar.</p><p><br /></p><h2 style="text-align: left;" id="repositori">Repositori</h2><p><b>Repositori</b> ialah struktur data yang menyimpan metadata untuk sekumpulan struktur berkas atau direktori.&nbsp; <i>rangkaian informasi</i> dalam repositori dapat diduplikasi pada sistem setiap pengguna atau dapat dipelihara pada satu <i>peladen(server)</i>. Beberapa metadata yang ada di repositori antara lain adalah:</p><p><br /></p><p></p><ul style="text-align: left;"><li>Catatan riwayat perubahan dalam repositori.</li><li>Sekumpulan objek komit.</li><li>Sekumpulan referensi untuk objek komit yang disebut heads.</li></ul><p></p><p><br /></p><p><br /></p><p><br /></p><h2 style="text-align: left;" id="tutorial">Cara clone repository</h2><p></p><blockquote><p>git clone https://github.com/username/namarepository</p><p>cd namarepositori</p><p>git add --all</p><p>#cek error</p><p>git commit -m "fush"</p><p>#add email anda</p><p>git config --global user.email "emailgithub kalian"</p><p>git config --global user.name "username github kalian"</p><p>#cek error</p><p>git commit -m "fush"</p><p>git push origin master</p></blockquote><p></p><p><br /></p><h2 style="text-align: left;" id="perintah">Semua perintah dan penjelasannya</h2><p><br />  <h3>Cloning Projek</h3>  <table class="mytable"><tbody>  <thead>    <tr><th>perintah</th><th>penjelasan</th></tr>    <tr><td>git init</td>    <td>Inisialisasi repositori Git lokal</td></tr>    <tr><td>git clone ssh://git@github.com/[username]/[repository-name].git</td>    <td>Buat salinan lokal dari repositori jarak jauh</td></tr>  </thead>       </tbody></table><h3>Basic Snapshotting</h3>  <table class="mytable"><tbody>  <thead>    <tr><th>perintah</th><th>penjelasan</th></tr>    <tr><td>git status</td>    <td>Check status</td></tr>  <tr><td>git add [file-name.txt]</td>    <td>Add a file to the staging area</td></tr>     <tr><td>git add -A</td>    <td>Tambahkan semua file baru dan yang diubah ke area pementasan</td></tr>    <tr><td>git commit -m "[commit message]"</td>    <td>Lakukan perubahan</td></tr>    <tr><td>git rm -r [file-name.txt]</td>    <td>Hapus file (atau folder)</td></tr>  </thead>       </tbody></table><h3>Percabangan & Penggabungan</h3>  <table class="mytable"><tbody>  <thead>    <tr><th>perintah</th><th>penjelasan</th></tr>    <tr><td>git branch</td>    <td>Daftar cabang (tanda bintang menunjukkan cabang saat ini)</td></tr>  <tr><td>git branch -a</td>    <td>Cantumkan semua cabang (lokal dan jarak jauh)</td></tr>     <tr><td>git branch [branch name]</td>    <td>Hapus cabang</td></tr>    <tr><td>git push origin --delete [branch name]</td>    <td>Hapus cabang jarak jauh</td></tr>    <tr><td>git checkout -b [branch name]</td>    <td>Buat cabang baru dan alihkan ke sana</td></tr>    <tr><td>git checkout -b [branch name] origin/[branch name]</td>    <td>Gandakan cabang jarak jauh dan alihkan ke sana</td></tr>   <tr><td>git branch -m [old branch name] [new branch name]</td>    <td>Beralih ke cabang</td></tr><tr><td>git checkout -</td>    <td>Beralih ke cabang yang terakhir diperiksa</td></tr>   <tr><td>git checkout -- [file-name.txt]</td>    <td>Buang perubahan ke file</td></tr><tr><td>git merge [branch name]</td>    <td>Gabungkan cabang menjadi cabang aktif</td></tr>   <tr><td>git merge [source branch] [target branch]</td>    <td>Gabungkan cabang menjadi cabang target</td></tr><tr><td>git stash</td>    <td>Simpan perubahan di direktori kerja kotor</td></tr>   <tr><td>git stash clear</td>    <td>Hapus semua entri yang disimpan</td></tr>  </thead>       </tbody></table><h3>Berbagi & Memperbarui Proyek</h3>  <table class="mytable"><tbody>  <thead>    <tr><th>perintah</th><th>penjelasan</th></tr>    <tr><td>git push origin [branch name]</td>    <td>Dorong cabang ke repositori jarak jauh Anda</td></tr>  <tr><td>git push -u origin [branch name]</td>    <td>Dorong perubahan ke repositori jarak jauh (dan ingat cabangnya) git push</td></tr>     <tr><td>git push</td>    <td>Mendorong perubahan ke repositori jarak jauh (cabang yang diingat)</td></tr>    <tr><td>git push origin --delete [branch name]</td>    <td>Hapus cabang jarak jauh</td></tr>    <tr><td>git pull</td>    <td>Perbarui repositori lokal ke komit terbaru</td></tr>    <tr><td>git pull origin [branch name]</td>    <td>Tarik perubahan dari repositori jarak jauh</td></tr>   <tr><td>git remote add origin ssh://git@github.com/[username]/[repository-name].git</td>    <td>Tambahkan repositori jarak jauh</td></tr><tr><td>git remote set-url origin ssh://git@github.com/[username]/[repository-name].git</td>    <td>Setel cabang asal repositori ke SSH</td></tr>  </thead>       </tbody></table> <h3>Basic Snapshotting</h3>  <table class="mytable"><tbody>  <thead>    <tr><th>perintah</th><th>penjelasan</th></tr>    <tr><td>git log</td>    <td>Lihat perubahan</td></tr>  <tr><td>git log --summary</td>    <td>Lihat perubahan (rinci)</td></tr>     <tr><td>git log --oneline</td>    <td>Lihat perubahan (secara singkat)</td></tr>    <tr><td>git diff [source branch] [target branch]</td>    <td>Pratinjau perubahan sebelum menggabungkan</td></tr>  </thead>       </tbody></table></p><p><br /></p><p><br /></p><h2 style="text-align: left;">Kesimpulan</h2><p>Terimakasih telah membaca sampai akhir. Semoga berguna dan selamat mencoba. Semoga berhasil.&nbsp;</p><p><br /></p><h2 style="text-align: left;">Pendapatmu</h2><p>Apakah penjelasan diatas membingungkan? Sudahkah kalian mencobanya? Jangan sungkan-sungkan untuk hubungi saya atau melalui komentar dibawah.</p><p><br /></p><p>Silahkan beri tanggapan, saran, kritik dan jika berkenan bisa follow media sosial saya. Kalian juga bisa request pembahasan berikutnya dikolom komentar dibawah.</p><p><br /></p><p>Terimakasih~</p><div><br /></div><p>Source :&nbsp;</p><p></p><ul style="text-align: left;"><li>https://id.wikipedia.org/</li><li>https://guides.github.com/</li><li>https://akhmadsyarif04.github.io/</li><li>https://id.bitdegree.org/</li></ul><p></p>
{{< /html >}}