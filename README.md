### TUGAS 7
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

### TUGAS 8
## Jelaskan perbedaan Navigator.push dan Navigator.pushReplacement.
Navigator.pushReplacement merupakan metode push yang membuang rute sebelumnya sehingga jika berpindah halaman tidak dapat kembali ke halaman sebelumnya. Navigator.push merupakan metode push untuk menambahkan rute lain ke atas tumpukan, jadi menampilkan halaman baru dan tetap dapat mengakses halaman sebelumnya.

## Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
ListTile adalah untuk menampilkan detail dari sebuah children. ListView adalah untuk menampilkan list dengan jumlah data yang besar.Form adalah untuk membukus form field. DropdownButton adalah untuk membuat button pilihan. SizedBox adalah untuk mengatur ukuran box. Drawer adalah untuk navigasi antar page.


## Sebutkan jenis-jenis event yang ada pada Flutter (contoh: onPressed).
onChanged adalah untuk mengeksekusi jika sebuah widget diubah. onFocusChanged adalah untuk mengeksekusi jika fokus berubah. onSaved adalah untuk mengeksekusi jika sebuah widget disiimpan. onHover adalah untuk mengeksekusi jika pointer bergerak dalam sebuah widget. onPressed adalah untuk mengeksekusi jika sebuah widget diklik.


## Jelaskan bagaimana cara kerja Navigator dalam "mengganti" halaman dari aplikasi Flutter.
Navigator pada flutter serupa dengan implementasi stack. Sehingga jika melakukan "push" akan menuju suatu halaman dan untuk mengembalikannya menggunakan "pop". "push" menambahkan halaman pada antrian teratas stack dan "pop" mengurangi halaman pada antrian stack.

## Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
Saya menambahkan drawer beserta dengan navigator mengarah ke class lain sesuai dengan ketentuan soal. Lalu, Saya membuat halaman form dengan membuat kelas pageform yang berisi textfield dan dropdown field, ketika submit di klik. Maka data form tersebut akan dijadikan instance dari model lalu disimpan pada ListModelBudget. lalu pada data_budget data di ListModelBudget di tampilkan.




## Tugas 9: Integrasi Web Service pada Flutter
## Apakah bisa kita melakukan pengambilan data JSON tanpa membuat model terlebih dahulu? Jika iya, apakah hal tersebut lebih baik daripada membuat model sebelum melakukan pengambilan data JSON?
Bisa saja, namun lebih baik menggunakan model dikarenakan dengan model mempresentasikan dari json. Selain itu, model dapat memastikan juga tipe data setiap field model dengan jelas. 

## Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
1. FutureBuilder = Untuk mengkontruksi widget berdasarkan snapshot.
2. Column = Mempresentasikan kolom
3. BoxDecoration = untuk mendekorasi elemen box flutter
4. FutureBuilder = membuat widget berdasarkan snapshot terakhir.

## Jelaskan mekanisme pengambilan data dari json hingga dapat ditampilkan pada Flutter.
Dilakukan dengan fetch pada method yang ada pada file, kemudian data di convert menjadi model dari json. Dari model tersebut disimpan dalam list, dan lalu tiap elemen dari list tersebut ditampilkan pada halaman.

## Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
Membuat model berdasarkan json yang akan diambil. Melakukan fetch dengan membuat Future async. Menampilkan data dari fungsi asinkronus.