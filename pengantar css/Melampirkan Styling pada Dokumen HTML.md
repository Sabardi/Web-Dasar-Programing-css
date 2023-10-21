# Setelah 
kita menuliskan rules, maka tahapan selanjutnya adalah melampirkan atau menerapkan aturan tersebut pada berkas HTML. Sebenarnya, terdapat tiga cara untuk menerapkan styling pada elemen HTML.

# External Style Sheet 

External Style Sheet merupakan berkas terpisah yang di dalamnya hanya terdapat sebuah rules. Berkas ini harus berekstensi .css, dan berkas ini nantinya dihubungkan pada dokumen HTML. Cara ini merupakan yang paling powerful dalam menerapkan styling. Karena dengan cara ini, satu berkas styling (.css) dapat digunakan oleh banyak berkas HTML.

Untuk menyambungkan berkas .css dengan dokumen HTML, kita dapat menggunakan elemen <link> pada <head> berkas HTML. Contohnya:
<head>
   <title>Document Title</title>
   <link rel="stylesheet" href="style.css">
</head>

Pada elemen <link> tersebut, kita tetapkan berkas CSS yang digunakan dengan menggunakan atribut href dan beri nilai “stylesheet” pada atribut rel sebagai relationship (hubungan) antara berkas style.css dengan dokumen HTML.

Pada contoh di atas kita tahu bahwa berkas css yang digunakan merupakan berkas lokal (berkas yang berada pada komputer/server kita sendiri). Nilai atribut href juga dapat berupa berkas .css yang tersedia melalui sebuah URL. 

Contohnya, banyak pengembang menggunakan bootstraps.min.css untuk membantu penyusunan layout website-nya. Kita bisa menggunakannya pada berkas HTML dengan langsung menuliskan URL untuk berkas tersebut.

<head>
   <title>Document Title</title>
   <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css">
</head>

min.css merupakan penamaan format berkas .css yang sudah di-minify atau sudah diminimalkan dengan menghilangkan white space yang tidak digunakan

# Embedded Style Sheet
Embedded Style Sheet merupakan kumpulan rules yang dituliskan dalam berkas HTML dengan menggunakan elemen <style>. Dengan begitu rules yang dituliskan hanya dapat dicakup oleh satu berkas HTML. Penulisan rules harus dituliskan dalam elemen <style> dan ditempatkan di dalam <head> dari berkas HTML.

<head>
   <title>Document Title</title>
   <style>
       /*
        * Rules styling dituliskan di sini
        */
   </style>
</head>

# Inline Style

inline Style merupakan styling yang diterapkan pada elemen HTML dengan menggunakan atribut style. Contohnya seperti berikut:

Untuk menambahkan styling properties lainnya (multiple properties), kita tuliskan dengan menggunakan semicolon (;) sebagai pemisah antar styling properties-nya.
<h1 style="color: green; margin-top: 2em">Kota Bandung</h1>

Inline styles hanya diterapkan pada elemen di mana atribut style diterapkan. Teknik ini seharusnya dihindari terkecuali benar-benar diperlukan untuk menggantikan sebuah styling yang ditetapkan pada Embedded Style Sheet atau External Style Sheet.


# Commenting in Style
Pada contoh kode di atas, kita sudah melihat sebuah teks pada rule yang dimulai dari /* dan diakhiri dengan */. Teks tersebut merupakan commenting line di dalam sebuah CSS. Sama seperti commenting pada HTML dan bahasa pemrograman lainnya, Teks yang dijadikan sebuah komentar tidak akan diproses oleh browser (sebagai compiler) atau lebih tepatnya “diabaikan”.


