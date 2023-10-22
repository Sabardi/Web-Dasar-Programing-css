# Pseudo Selector
Selain beberapa selector yang sudah kita pelajari, CSS masih memiliki dua selector lagi yang dapat kita manfaatkan untuk membantu menyeleksi elemen dalam menerapkan sebuah rule, yakni pseudo-class dan pseudo-element.

Sebelum menjelaskan lebih detail tentang kedua selector tersebut, perlu kita ketahui pseudo selector berbeda dari selector yang sudah dibahas sebelumnya. Selector ini menargetkan elemen pada bagian yang “tidak terlihat”, seperti sifat pada elemen sehingga untuk menetapkannya tidak bisa menggunakan selector biasa. Salah satu contoh yang paling sering kita terapkan adalah :hover, pseudo selector tersebut kita gunakan untuk menetapkan rule ketika cursor diarahkan ke target elemen.

a:hover {
  color: blue;
}

Contoh kode di atas merupakan salah satu pseudo-class selector, yang menyebabkan elemen anchor menerapkan warna biru ketika kursor diarahkan pada elemen tersebut.

Mari kita bahas lebih detail mengenai pseudo-class selector dan pseudo-element selector.

