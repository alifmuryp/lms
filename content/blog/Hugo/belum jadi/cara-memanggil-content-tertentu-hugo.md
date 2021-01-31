---
title: "8 Syntax Yang Perlu Kalian Pahami untuk Memanggil Konten atau Variabel"
slug: 8-bassic-syntax
date: 2021-01-23T09:48:42Z
draft: false 
authors:
 - MuryP
show_comments: true 
 
type: pages 
 
tags: 
- Hugo
- Template


  
  
 
description: "Cara memanggil konten tertentu untuk mempermudah management konten." 
keywords: "Cara memanggil konten tertentu untuk mempermudah management konten." 
--- 
Hello world!
Kali ini kita akan membahas salah satu syntax bassic yang saya gunakan untuk membuat template ini dan lainnya. Oh dan mungkin akan ada beberapa update nantinya seiring penggunaan hugo. Karena saya baru saja menggunakan Hugo, maka aku tak banyak tahu mengenai syntax yang ada. Namun setidaknya dengan beberapa syntax berikut bisa kalian pelajari untuk membuat template kalian sendiri.

1. Tanda kurung Pada Hugo 

Jika kalian sudah mempelajari bahasa **golang** atau bahasa lainnya. Kalian sudah tidak asing dengan yang namanya `{{ }}` dinama kita bisa menggunakan untuk memanggil konten. Jika di JS maka kita sering menggunakan untuk membungkus element yang panjang. Namun untuk di Hugo itu agak berbeda. Kita akan membahasnya di nomor selanjutnya.

2. Memberikan judul di Hugo 

Umumnya saat kita ingin memanggil judul maka kita bisa menggunakan `{{ .Title }}` meskipun kita bisa menggunakan params juga untuk memanggilnya. Namun cara ini yang paling singkat

3. Memanggil variabel dalam kode

Nah ini kebanyakan bahasa mempunyai ini, kita hanya perlu mendefinisikan sebuah variabel yang nantinya bisa kita panggil berulang-ulang. Contohnya berikut :
```
{{ $rumah := .Site.Params }}
{{ $warna2 := $rumah.warna2 }}
// cara memanggilnya
{{ $rumah }}
// juga bisa digabung
{{ $muda := $rumah.muda }}
```
keterangan :
disini kita lihat kita tak perlu menulis kode sama yang panjang berkali-kali, kita hanya perlu mendefinisikan lalu memanggilnya. Meskipun yang saya gunakan itu gak telalu panjang, tapi biar lebih mudah dan rapi nantinya, kita bisa menggunakannya. Dan setahu saya ini dilakukan jika satu file saja.

4. Memanggil Params 

Bagi kalian yang belum tahu apa itu params, saya akan menjelaskan sedikit. Secara awam, Params mirip dengan sebelumnya. Berbeda dengan sebelumnya, Params bisa dipanggil di berbagai file manapun. Dimana kita bisa membuatnya di config.toml dan sebelum artikel. Mulai dari nama situs, judul, deskripsi, sampai kita bisa membuat apapun yang nantinya bisa kita panggil dimana saja. 

isi config.toml dengan
```
title = "MuryP Studio"
```
lalu untuk memanggilnya
```
{{ Site.Title }}
```


5. Menampilkan jumlah konten pada section tertentu, biasanya diawali dengan deklarasi section.
```
 {{ len .RegularPages }}
```

6. Menampilkan format tanggal

Untuk menampilkan format tanggal kita bisa mendeklarasikan terlebih dahulu mana yang akan ditampilkan tanggalnya. Disini saya menggunakan untuk menampilkan tanggal berapa postingan ini dibuat. 

- menampilkan tanggal berapa

```
<span class="day">{{ dateFormat "02" .Date }}</span>
```

- Dibawah ini kita bisa lihat jika saya mempunya konfigurasi mengenai tanggal dan bulan maka akan ditampilkan, namun jika tidak maka format tanggal akan diubah seperti "Jan 2006" meskipun nantinya yang tampil akan sesuai postingan.
      
```
<span class="rest">
{{ if $.Site.Data.month }}{{ index $.Site.Data.month (printf "%d" .Date.Month) }} {{ .Date.Year }}{{ else }}{{ dateFormat "Jan 2006" .Date }}{{ end }}</span>
```
7. Membuat menu di Hugo 
Untuk memudahkan kita membuat menu, kita bisa menggunakan cara berikut, yang nantinya akan saya bahas lebih lengkap nantinya [disini](/menus-di-hugo).


Pertama kalian bisa isi terlebih dahulu config.toml nya
```
[menu]
  [[menu.main]]
    identifier = "Home"
    name = "Home"
    url = "/"
    weight = 1
#dibawah ini wilayah sosmed
  [[menu.sosmed]]
    identifier = "About"
    name = "About"
    url = "/about/"
    weight = 1
```
lalu kalian bisa memanggilnya dengan cara
```html
{{ range .Site.Menus.sosmed.Sort.ByWeight }}
<a href='{{ .URL }}' rel='nofollow' target='_blank' title='{{ .Name }}'>
<span class='{{ .Name }}' /></a>
{{ end }}
```

8. Partial Hugo

Untuk memudahkan kita untuk membuat blog, kita bisa memisahkan kode menjadi beberapa, yang nantinya disatukan menjadi satu. Hal ini sama seperti saat kita menggunakan javascript atau php juga ada atau bahasa lainnya. Entahlah, saya lupa namanya, tapi saya pernah melihat hal yang sama di php dan javascript. Dan untuk hugo sendiri kita mudah menggunakan partial. Kita hanya perlu membuat file baik itu berekstensi HTML,JS maupun CSS di folder themes/nameThmes/layout/partial dan memanggilnya atau menyatukan di index.html ataupun di _default untuk list dan post. Yang dimana akan saya bahas lebih lengkap [disini](/partial-hugo)

```
  {{ partial "folder1/subfolder1/file.html" . }}
  // atau
  {{ partial "file.html" . }}
```
keterangan :
karena disini saya mempunyai banyak partial, maka saya membuat beberapa folder untuk merapikannya. 

> jika ada kode lainnya akan ditulis dibawah :

## Kesimpulan 

Penggunaan hugo itu sangat cocok bagi pemula ketimbang yang lainnya. Meskipun untuk pemasangannya sendiri itu agak ribet, tapi kita bisa lebih mudah untuk mengembangkan template. Meskipun tidak ada GUI seperti Blogger dan Wordpress. Namun Bagi kalian yang belaja di HP saya sarankan belajar HUGO dulu, biar gak terlalu pusing dengan xml dan javascript yang ada pada cms yang saya sebutkan tadi. 

## Pendapatmu 

Lalu apa pendapatmu  mengenai Hugo ini? Apakah syntax tersebut mudah kalian mengerti? jika tidak, mana bagian yang belum anda mengerti? silahkan tulis di kolom komentar dibawah. 

Sekian dari saya, jika ada salah kata atau hal yang membingungkan. Semoga bermanfaat dan terus belajar serta berkarya lebih baik lagi. Jika kalian suka dengan materi tersebut silahkan share ke teman kalian, kalian juga bisa menyalin seluruh isi artikel dan menyimpannya secara local melalui github atau gitlab. Kalian juga bisa membantu saya mengembangkan blog ini dengan memperbaiki kata atau kode yang telah kubuat. Jika ingin tahu mengenai perkembangan mengenai blog ini silahkan follow sosial media saya. 

Sekian terimakasih