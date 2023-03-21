# Lab2Web.
Melakukan install pada XAMPP
Download XAMPP terbaru melalui website Apache Friends https://www.apachefriends.org/index.html

Lakukan instalasi setelah Anda selesai mengunduh. Selama proses instalasi mungkin Anda akan melihat pesan yang menanyakan apakah Anda yakin akan menginstalnya. Silakan tekan Yes untuk melanjutkan instalasi. Setelah itu kalian dapat melakukan Extract File tersebut dengan menyesuaikan lokasi penyimpanannya seperti gambar dibawah.
![Screenshot (124)](https://user-images.githubusercontent.com/93463612/226530950-47cc1cb4-7722-4fbc-8b62-cda65cbd4115.png)


proses menjalankan xampp
Untuk dapat menjalankan Xampp ini kalian perlu membukanya terlebih dulu, setelah itu kalian klik tombol start pada bagian server Apache, dan tampilan utama Xampp seperti gambar dibawah ini jika berhasil.
![Screenshot (121)](https://user-images.githubusercontent.com/93463612/226530887-513d7a60-bce3-44e5-abc3-6923dcbfad7d.png)

MEMULAI PHP
Pertama, buatlah folder Lab7_php_dasar pada root directory web server (c:xampp/htdocs)

PHP DASAR
![Screenshot (127)](https://user-images.githubusercontent.com/93463612/226532725-6262d1e3-5361-4143-b9f2-617c72cb88d3.png)

Untuk dapat mendapatkan tampilan seperti gambar diatas, buatlah file baru dengan nama php_dasar.php pada directory tersebut. Kemudian tambahkan kode berikut:
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>PHP Dasar</title>
</head>

<body>
    <h1>Belajar PHP Dasar</h1>
    <?php
    echo "Hello World";
    ?>
</body>

VARIABLE PHP
![PhpDasar](https://user-images.githubusercontent.com/93463612/226531281-31b1a58a-c265-46f2-ad06-7d782b391d30.png)

Untuk mendapatkan tampilan seperti diatas kalian bisa menambahkan kode berikut:
  <!DOCTYPE html>
<html lang="en">
  <body>
    <h1>Menggunakan Variabel</h1>
    <?php
    $nim = "312110322";
    $nama = 'Choky Andriano';
    echo "NIM : " . $nim . "<br>";
    echo "Nama : $nama";
    ?>
</body>

</html>

PREDEFINE $_GET
Buatlah file baru dalam Directory Lab_php_dasar dengan nama file disini saya namakan dengan latihan2.php 
![PredifineVariable](https://user-images.githubusercontent.com/93463612/226531398-0e4cdaed-4fc0-449c-bca1-a8ea432d0f16.png)

dan untuk mengaksesnya dapat menggunakan URL : http://localhost/lab2_php_dasar/latihan2.php?nama=Choky
Berikut kode yang digunakan
<body>
    <h1>Predifine Variable</h1>
    <?php
    echo 'Selamat Datang ' . $_GET['nama'];
    ?>
</body>
  
PEMBUATAN FORM INPUT DENGAN VARIABLE $_POST
![FormInput](https://user-images.githubusercontent.com/93463612/226531461-0cce662a-4ee5-4bfd-b88a-f7c8b9921896.png)

berikut kode untuk tampilan diatas:
 <!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>PHP Dasar</title>
</head>

<body>
    <h2>Form Input</h2>
    <form method="post">
        <label>Nama: </label>
        <input type="text" name="nama">
        <input type="submit" value="Kirim">
    </form>
    <?php
    echo 'Selamat Datang ' . $_POST['nama'];
    ?>
</body>

</html>

OPERATOR
![Operator](https://user-images.githubusercontent.com/93463612/226531497-24abfc8c-fe34-49c5-a752-86f4a7c25eaa.png)

Untuk mendapat tampilan diatas, buatlah file baru dengan nama file disini saya namakan Operator.php dalam directory lab2_php_dasar. Kemudian tambahkan kode berikut:
  <?php
$gaji = 1000000;
$pajak = 0.1;
$thp = $gaji - ($gaji*$pajak);
echo "Gaji sebelum pajak = Rp. $gaji <br>";
echo "Gaji yang dibawa pulang = Rp. $thp";

KONDISI IF
![KondisiIF](https://user-images.githubusercontent.com/93463612/226531556-827d71d1-9e3a-49f8-9909-b37864462a40.png)

Untuk mendapat tampilan pengkondisian IF ELSE seperti diatas, buatlah file baru dengan nama file disini saya namakan KondisiIF.php dalam directory lab2_php_dasar. Kemudian tambahkan kode berikut:

<?php
$nama_hari = date("l");
if ($nama_hari == "Sunday") {
 echo "Minggu";
} elseif ($nama_hari == "Monday") {
 echo "Senin";
} else {
 echo "Selasa";
}


KONDISI SWITCH
![Screenshot (123)](https://user-images.githubusercontent.com/93463612/226532048-0a9df8e3-98d6-459a-aa76-c46ecf7ed25d.png)

Untuk mendapat tampilan pengkondisian SWITCH CASE dengan break seperti diatas, buatlah file baru dengan nama file disini saya namakan KondisiSwitch.php dalam directory lab2_php_dasar. Kemudian tambahkan kode berikut:
<?php
$nama_hari = date("l");
switch ($nama_hari) {
 case "Sunday":
 echo "Minggu";
 break;
 case "Monday":
 echo "Senin";
 break;
 case "Tuesday":
 echo "Selasa";
 break;
 default:
 echo "Sabtu";
 }
 ?>
  
PERULANGAN FOR
![PerulanganFor](https://user-images.githubusercontent.com/93463612/226532136-fe6b62bd-f868-4d5b-8688-6a1a71d1d789.png)

Untuk mendapat tampilan seperti diatas, buatlah file baru dengan nama file disini saya namakan PerulanganFor.php dalam directory lab2_php_dasar. Kemudian tambahkan kode berikut:
<?php
echo "Perulangan 1 sampai 10 <br />";
for ($i=1; $i<=10; $i++) {
 echo "Perulangan ke: " . $i . '<br />';
}
echo "Perulangan Menurun dari 10 ke 1 <br />";
for ($i=10; $i>=1; $i--) {
 echo "Perulangan ke: " . $i . '<br />';
}
?>
  
PERULANGAN WHILE
![PerulanganWhile](https://user-images.githubusercontent.com/93463612/226532168-cce080e4-f237-4830-a8dd-26c13db13453.png)
Untuk mendapat tampilan seperti diatas, buatlah file baru dengan nama file disini saya namakan  PerulanganWhile.php dalam directory lab2_php_dasar. Kemudian tambahkan kode berikut:

  <?php
echo "Perulangan 1 sampai 10 <br />";
$i=1;
while ($i<=10) {
 echo "Perulangan ke: " . $i . '<br />';
 $i++;
}
?>
  
PERULANGAN DOWHILE
![PerulanganDowhile](https://user-images.githubusercontent.com/93463612/226532219-aee0af53-b3ce-4862-a4c8-e41c9749fde9.png)

Untuk mendapat tampilan seperti diatas, buatlah file baru dengan nama file disini saya namakan PerulanganDowhile.php dalam directory lab2_php_dasar. Kemudian tambahkan kode berikut:

  <?php
echo "Perulangan 1 sampai 10 <br />";
$i=1;
do {
 echo "Perulangan ke: " . $i . '<br />';
 $i++;
} while ($i<=10);
?>
  
PERTANYAAN DAN TUGAS
Buatlah program PHP sederhana dengan menggunakan form input yang menampilkan nama , tanggal lahir dan pekerjaan . Kemudian tampilkan outputnya dengan menghitung umur berdasarkan inputan tanggal lahir . Dan pilihan pekerjaan dengan gaji yang berbeda-beda sesuai pilihan pekerjaan.
![Tugas3](https://user-images.githubusercontent.com/93463612/226532245-f0916582-ed30-4d09-934a-440dc3373c43.png)
