# Tugas-Tic-Tac-Toe
Praktikum 6 Permainan Tic Tac Toe Program menggunakan module "tkinter" dalam bahasa pemrograman phyton. Berikut penjelasan mengenai setiap bagian program
1. Program dimulai dengan mengimpor modul 'tkinter' dengan alias 'tk', yang digunakan untuk membuat Graphical User Interface (GUI).

![1](https://github.com/SaktiaWardhana/Tugas-Tic-Tac-Toe/assets/148610993/0f5aef0c-7b1c-41d6-bed3-d35e2acc664e)

2. Kelas 'GameState' didefinisikan untuk menggambarkan status permainan, termasuk 
- PLAYING (sedang berlangsung)
- DRAW (seri)
- CROSS_WON (X menang)
- NOUGHT_WON (O menang)

![2](https://github.com/SaktiaWardhana/Tugas-Tic-Tac-Toe/assets/148610993/1cbf03b0-c871-47fe-99ed-8db4847818bb)

3. Kelas 'Seed' digunakan untuk mewakili isi sel dalam papan permainan, dengan tiga kemungkinan nilai:
- EMPTY (kosong)
- CROSS (X)
- NOUGHT (O)

![3](https://github.com/SaktiaWardhana/Tugas-Tic-Tac-Toe/assets/148610993/c1d28180-3438-4bb9-93b1-a97544543967)

4. Kelas 'Cell' menggambarkan sel dalam papan permainan dan memiliki atribut seperti:
- content (isi sel)
- row (baris sel)
- col (kolom sel)

![4](https://github.com/SaktiaWardhana/Tugas-Tic-Tac-Toe/assets/148610993/318936d0-4cbb-4396-8bc6-68ba3cfabcb4)

Kelas ini memiliki metode:
clear : untuk mengosongkan sel
paint : untuk menggambar sel di elemen canvas menggunakan tkinter. Sel yang berisi "X" digambar dengan garis-garis merah, dan sel yang berisi "O" digambar dengan lingkaran biru.

![5](https://github.com/SaktiaWardhana/Tugas-Tic-Tac-Toe/assets/148610993/be3dc7d1-c998-46f4-8288-299511e31408)

5. Deklarasi Kelas Board
   Kelas Board digunakan untuk menggambarkan papan permainan Tic-Tac-Toe dan memiliki atribut berupa matriks 3x3 yang disebut 'cells' yang terdiri dari objek-objek Cell. Kelas Board dilengkapi dengan beberapa metode sebagai berikut:
- Metode 'init' digunakan untuk mengosongkan sel-sel di papan permainan pada awal permainan.
- Metode 'is_draw' berguna untuk memeriksa apakah permainan telah berakhir seri, yang terjadi ketika semua sel di papan telah terisi.
- Metode 'has_won' digunakan untuk mengecek apakah ada pemain yang telah memenangkan permainan dengan memeriksa baris, kolom, atau diagonal pada papan permainan.
- Metode 'paint' digunakan untuk menggambar papan permainan ke dalam elemen canvas dengan bantuan objek Cell. Pada saat menggambar, sel-sel dengan isi "X" akan digambarkan dengan garis-garis merah, sedangkan sel-sel dengan isi "O" akan digambarkan sebagai lingkaran biru.

![6](https://github.com/SaktiaWardhana/Tugas-Tic-Tac-Toe/assets/148610993/1c26cee6-7280-4016-9238-bba950204f26)

6. Deklarasi Kelas GameMain
   Kelas GameMain merupakan kelas utama dalam program yang bertanggung jawab atas pengaturan permainan dan tampilan antarmuka grafis (GUI). Kelas ini memiliki beberapa atribut konstan yang digunakan untuk mengatur tampilan, seperti ukuran sel, lebar garis, dan elemen-elemen lainnya. Kelas GameMain dilengkapi dengan beberapa metode sebagai berikut:
- Metode '_ _init _ _' digunakan untuk melakukan inisialisasi GUI dan papan permainan pada saat program dijalankan.
- Metode 'init_game' bertujuan untuk memulai permainan dengan mengosongkan sel-sel di papan permainan, sehingga permainan dimulai dari awal.
- Metode 'update_game' digunakan untuk memeriksa apakah terdapat pemain yang telah memenangkan permainan atau apakah permainan telah berakhir seri. Ini adalah langkah penting dalam memeriksa hasil permainan.
- Metode 'paint' berfungsi untuk menggambar tampilan papan permainan ke dalam elemen canvas pada antarmuka grafis. Dengan metode ini, seluruh elemen permainan akan ditampilkan kepada pemain.
- Metode 'handle_click' digunakan untuk menangani tindakan klik mouse dari pengguna. Metode ini akan mengisi sel di papan permainan dengan "X" atau "O" sesuai dengan giliran pemain saat itu. Jadi, jika giliran pemain pertama, sel akan diisi dengan "X," dan jika giliran pemain kedua, sel akan diisi dengan "O."

![7](https://github.com/SaktiaWardhana/Tugas-Tic-Tac-Toe/assets/148610993/0194c4f8-d4b1-4eaa-9734-2f11b9f16df8)

7. Program membuat instance dari kelas 'Tk' dari modul tkinter sebagai root window.

![8](https://github.com/SaktiaWardhana/Tugas-Tic-Tac-Toe/assets/148610993/c539b9e6-32e6-443e-a5f4-498a5f48868d)

8. Program membuat instance dari kelas 'GameMain' menggunakan root window sebagai parent.

![9](https://github.com/SaktiaWardhana/Tugas-Tic-Tac-Toe/assets/148610993/498a7707-dbb3-41cb-aed1-9e829b084e2b)

9. Binding Event Click
    Program mengikat event klik mouse kiri ke metode 'handle_click'.
   
![10](https://github.com/SaktiaWardhana/Tugas-Tic-Tac-Toe/assets/148610993/bdb9626b-b880-4ccd-bae7-c0b5b1e7a32c)

10. Memulai Loop Utama
    Program memulai loop utama GUI dengan memanggil 'mainloop()', yang mengurus interaksi pengguna dan pembaruan tampilan permainan.

![11](https://github.com/SaktiaWardhana/Tugas-Tic-Tac-Toe/assets/148610993/088d7c38-74cc-46ed-863e-bacb1e7feea1)


Program ini menciptakan permainan Tic-Tac-Toe dengan antarmuka GUI, memungkinkan pemain untuk bermain dan memeriksa hasil permainan melalui elemen canvas yang digambar menggunakan tkinter.

![12 tic tac toe](https://github.com/SaktiaWardhana/Tugas-Tic-Tac-Toe/assets/148610993/f9adb7d1-909c-4332-b5cd-ab8f15957136)





