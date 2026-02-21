# Tugas Proyek WEB 3
<p>Pada tugas ini, saya membuat sebuah program menggunakan bahasa pemrograman JavaScript yang dijalankan melalui Node.js (tanpa menggunakan HTML). Program ini bertujuan untuk menentukan zodiak seseorang berdasarkan tanggal dan bulan lahir yang diinput oleh pengguna.</p>


<h2>📌 Penjelasan Kode</h2>
<h3>1️⃣ Mengimpor Module readline<h3>
<pre> const readline = require("readline"); </pre>
<p>Baris ini digunakan untuk mengimpor module bawaan Node.js yaitu readline.
  Module ini berfungsi agar program dapat menerima input dari pengguna melalui terminal.</p>
  
<h3>2️⃣ Membuat Interface Input dan Output<h3>
<pre> const rl = readline.createInterface({
      input: process.stdin,
      output: process.stdout
      });</pre>
<p>Kode ini membuat koneksi antara program dan terminal.
  process.stdin digunakan untuk menerima input, sedangkan process.stdout untuk menampilkan output.</p>

<h3>3️⃣ Membuat Fungsi tentukanZodiak<h3>
<pre> function tentukanZodiak(tanggal, bulan) { </pre>
<p>Fungsi ini dibuat untuk menentukan zodiak berdasarkan tanggal dan bulan lahir.
  Nilai tanggal dan bulan akan dikirim sebagai parameter saat fungsi dipanggil.</p>

<h3>4️⃣ Percabangan If-Else<h3>
<pre> if ((bulan == 3 && tanggal >= 21) || (bulan == 4 && tanggal <= 19)) {
      return "Aries";
      } </pre>
<p>Bagian ini menggunakan percabangan untuk mengecek rentang tanggal setiap zodiak.
  Jika kondisi terpenuhi, maka fungsi akan mengembalikan nama zodiak yang sesuai.</p>

<h3>5️⃣ Mengambil Input dari User<h3>
<pre> rl.question("Masukkan tanggal lahir (1-31): ", function (tanggal) { </pre>
<p>Kode ini digunakan untuk menampilkan pertanyaan dan menerima jawaban dari pengguna.
  Jawaban yang dimasukkan akan disimpan ke dalam variabel untuk diproses lebih lanjut.</p>

<h3>6️⃣ Mengubah Input Menjadi Angka<h3>
<pre> tanggal = parseInt(tanggal);
      bulan = parseInt(bulan); </pre>
<p>Input dari terminal berbentuk teks (string), sehingga perlu diubah menjadi angka.
  Hal ini dilakukan agar bisa dibandingkan dengan angka pada proses percabangan.</p>

<h3>7️⃣ Menampilkan Output<h3>
<pre> console.log("Tanggal Lahir:", tanggal + "/" + bulan);
      console.log("Zodiak:", zodiak); </pre>
<p>Kode ini digunakan untuk menampilkan hasil akhir ke terminal.
  Program akan menampilkan tanggal lahir yang dimasukkan serta zodiak yang sesuai.</p>

<h2>📸 Screenshot Percobaan</h2>
<img width="443" height="343" alt="image" src="https://github.com/user-attachments/assets/f55e3bbd-bf74-4272-b972-a202fd314b26" />
