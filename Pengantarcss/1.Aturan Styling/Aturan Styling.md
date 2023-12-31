# Menuliskan Aturan Styling
Sebuah style sheet terdiri dari satu atau lebih aturan styling (biasa disebut dengan rules atau rule-sets) yang mendeskripsikan bagaimana sebuah elemen atau sebuah kelompok elemen ditampilkan dalam jendela browser. 

Langkah awal belajar CSS adalah dengan memahami sebuah bagian rule. Berikut ini dua contoh rules yang dituliskan dalam sebuah CSS. Rule yang pertama menetapkan sebuah warna hijau pada elemen <h1> dan rule yang kedua menetapkan ukuran font dan tipe font pada sebuah elemen paragraf.

h1 { color: green; }
 
p {
   font-size: small;
   font-family: sans-serif;
}

Dalam penggunaan CSS, terdapat dua bagian dalam sebuah rule. Yang pertama adalah identitas elemen atau elemen yang akan menerapkan rule (singkatnya kita akan sebut selector) dan yang kedua adalah deklarasi atau instruksi yang akan diterapkan pada sebuah selector.

![Alt text](image.png)

# Selector
Pada contoh di atas, h1 dan p digunakan sebagai selector. Selector ini dipanggil melalui tipe elemennya, dan ini merupakan teknik dasar dari pemanggilan selector. Properti dan nilainya yang terdapat pada declaration/declaration block akan diterapkan pada seluruh elemen <h1> dan <p> yang ada pada dokumen HTML. Pada sub-modul selanjutnya kita akan mengetahui berbagai cara lainnya untuk menetapkan selector dengan lebih canggih lagi.

# Declarations
Bagian deklarasi terdiri dari pasangan properti dengan nilainya. Kita bisa menetapkan lebih dari satu deklarasi pada satu rule, contohnya seperti pada selector p di atas. Kita menetapkan lebih dari satu deklarasi pada declaration block. Setiap deklarasinya harus diakhiri dengan semicolon (;) sebagai tanda diakhirinya sebuah deklarasi.

Karena CSS tidak memperhatikan spasi (sama seperti bahasa pemrograman pada umumnya), sebaiknya penulisan deklarasi selalu diawali dengan baris baru supaya mudah dibaca dan dipahami.

p {
   font-size: small;
   font-family: sans-serif;
   /* deklarasikan nilai properti lainnya pada baris baru */
}

Tapi ingat, walaupun CSS tidak memperhatikan spasi, untuk satuan nilai seperti px, em, rem, dan lainnya harus dituliskan tanpa spasi pada nilainya. Contohnya:

h1 {
   margin: 2em;
}

Jika kita menambahkan spasi di antara satuan dan nilai, maka deklarasi tersebut tidak akan berfungsi.
h1 {
   margin: 2 em; /* Deklarasi tidak akan berfungsi karena terdapat spasi antara nilai dan satuan */
}

# CSS Comments
CSS comments digunakan untuk menjelaskan kode dan dapat membantu ketika Anda mengedit kode sumber di lain waktu. Apa yang tertulis akan diabaikan oleh browser dan tidak ditampilkan di browser, sehingga dapat menjadi opsi baik untuk memberi catatan atau informasi dokumentasi pada kode.

Seperti contoh yang beberapa kali telah Anda lihat diatas, CSS comments ditempatkan pada elemen <style> dengan cara penulisan dimulai dengan /* dan diakhiri */ seperti contoh berikut:
p {
   font-size: small;
   font-family: sans-serif;
   /* memilih sans-serif sesuai hasil diskusi klien pada 2 Jan 2021*/
}
