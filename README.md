# PHP6LavedaNafisArshanda
1. Jelaskan menggunakan bahasa sendiri perbedaan antara cookies dan session!

Cookies adalah informasi yang disimpan di dalam browser, cookies di deklarasikan sebelum tag <html>.
Session adalah sebuah variabel global yang di ciptakan di dalam server php, session di deklarasikan pada awal header sebelum tag <html>.
  
 2. Bagaimana cara menghapus session dan cookies pada sebuah browser!

a. Pilih tombol berbentuk “kunci inggris” pada sisi kanan atas.
b. Pilih “Tools”.
c. Pilih “Clear Browsing Data”.
d. Pilih “Cache dan Cookies”.
e. Pilih “Clear Browsing Data”

CARA CEPAT = Tekan (Ctrl + Shift + Del)
 
3. Berikan contoh kode dari pembuatan dan menghapus cookies dan session!

Membuat cookies :
 <?php  
// Men-set nilai cookie
 setcookie('nama_cookie', 'nilai_cookie'); 
 // Mendapatkan nilai cookie 
 echo $_COOKIE['nama_cookie'];
  ?>  
<p> 
  
Menghapus cookies :
<?php
       setcookie('nama_cookie', 'nilai_cookie'); 
 if (isset($_COOKIE['nama_cookie'])) { 
       echo 'cookie di-set <br />'; 
// Menghapus cookie, dengan masa berlaku 1 jam yang lalu 
setcookie('nama_cookie', '', time() - 1 * 3600);
  echo 'cookie dihapus';  
} else {  
     echo 'unset';
      } ?>  
  
Membuat session :
 <?php  
// Inisialisasi data session 
session_start();
 // Set session jika belum ada 
 if (!isset($_SESSION['test'])) { 
       $_SESSION['test'] = 'value'; 

} else { 
    echo 'Session di-set <br />'; 
    // Mencetak nilai session test
     echo 'Nilai: ' . $_SESSION['test'] . '<br />';  
  // Mencetak semua elemen session  
   print_r($_SESSION); 
   } 
   ?> 
   
Menghapus session :  
   if (isset($_SESSION['test'])) { 
                // Hapus session test 
unset($_SESSION['test']); 
  echo 'session dihapus';
   } else {  
        echo 'unset'; 
        
![alt text](https://github.com/LavedaNafisArshanda/PHP6LavedaNafisArshanda/blob/master/1.JPG)
![alt text](https://github.com/LavedaNafisArshanda/PHP6LavedaNafisArshanda/blob/master/2.JPG)
![alt text](https://github.com/LavedaNafisArshanda/PHP6LavedaNafisArshanda/blob/master/3.JPG)
![alt text](https://github.com/LavedaNafisArshanda/PHP6LavedaNafisArshanda/blob/master/4.JPG)
![alt text](https://github.com/LavedaNafisArshanda/PHP6LavedaNafisArshanda/blob/master/5a.JPG)
![alt text](https://github.com/LavedaNafisArshanda/PHP6LavedaNafisArshanda/blob/master/5b.JPG)
![alt text](https://github.com/LavedaNafisArshanda/PHP6LavedaNafisArshanda/blob/master/6a.JPG)
![alt text](https://github.com/LavedaNafisArshanda/PHP6LavedaNafisArshanda/blob/master/6b.JPG)
![alt text](https://github.com/LavedaNafisArshanda/PHP6LavedaNafisArshanda/blob/master/p1.JPG)
![alt text](https://github.com/LavedaNafisArshanda/PHP6LavedaNafisArshanda/blob/master/p3.JPG)
![alt text](https://github.com/LavedaNafisArshanda/PHP6LavedaNafisArshanda/blob/master/p4.JPG)
