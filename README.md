## Jelaskan apa yang dimaksud dengan stateless widget dan stateful widget dan jelaskan perbedaan dari keduanya.
- Widget stateless adalah widget yang tidak dapat diubah/tidak diubah (immutable). Konfigurasi yang dikandungnya diinisialisasi dari awal. Widget ini tidak mengubah data, jadi statis.
- Widget stateful adalah widget yang mudah berubah. Widget stateful dapat mengubah data sebagai respons terhadap interaksi pengguna. Untuk mengubah perubahan data, panggil fungsi setState() untuk memanipulasi dan mengubah data.
- Widget stateless dan stateful biasanya digunakan dalam file dart. Pada dasarnya, perbedaan yang cukup mencolok adalah bahwa widget stateless tidak dapat diubah, sedangkan widget stateful dapat diubah. Contoh widget stateless adalah Text, Icon dan IconButton. Contoh widget stateful termasuk Checkbox, Radio, dan TextField.

## Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
1. Text = Untuk menampilkan text.
2. FloatingActionButton = Instance action button.
3. Center = mengatur posisi supaya berada di tengah.
4. Column = mengatur layout secara vertikal.
5. MaterialApp = parent yang didalamnya menerapkan style material design.
6. Row = mengatur layout secara horizontal.
7. Scaffold = Untuk mengatur visual layout dengan mengimplementasikan material design.


## Apa fungsi dari setState()? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.
fungsi dimana dijalankan kode-kode yang biasanya akan merubah widget, dijalankan pada setiap pembaharuan.

## Jelaskan perbedaan antara const dengan final.
final diinialisasi pada saat pertama kali digunakan dan hanya di setting sekali. Final dapat digunakan untuk variabel immutable yang nilainya sudah/belum diketahui saat compile-time. const digunakan pada variabel immutable yang nilainya bersifat konstan. Const harus sudah diketahui pada saat waktu compile-time yang artinya nilai dari variabel tersebut sudah diberikan secara langsung. 

## Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
Membuat aplikasi flutter, lalu menambahkan floating action button untuk pengurangan disertai fungsi decrements. Lalu membuat text dan style text ganjil dan genap menyesuaikan terhadap angka. 