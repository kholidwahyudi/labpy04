# Buat program sederhana untuk menambahkan data kedalam sebuah list dengan rincian sebagai berikut:
###• Progam meminta memasukkan data sebanyak-banyaknya (gunakan perulangan)
###• Tampilkan pertanyaan untuk menambah data (y/t?), apabila jawaban t (Tidak), maka program akan menampilkan daftar datanya. • Nilai Akhir diambil dari perhitungan 3 komponen nilai (tugas: 30%, uts: 35%, uas: 35%)

## Flowchart
<img width="388" alt="3" src="https://user-images.githubusercontent.com/115494491/203001505-3a6a7789-4a9f-49f0-b516-9adb46e0d462.png">
Berikut tampilan program menggunakan bahasa Python :
<img width="960" alt="1" src="https://user-images.githubusercontent.com/115494491/203000807-b4cb71fe-331a-4120-9ce6-b86d85c5e90a.png">

1. from prettytable import PrettyTable Membuat header table menggunakan prettytable. Variabel import berfungsi untuk memanggil file lain di dalam satu module yang berbeda.

1. print("Program Input Data Mahasiswa") print() untuk menampilkan kalimat yang di input.
- tabelNama = PrettyTable(["No" ,"Nama" ,"NIM" ,"Nilai Tugas" ,"Nilai UTS" ,"Nilai UAS" ,"Nilai Akhir" ])
- a = 0
- (Deklarasi list)untuk menginput data yang dimasukkan kedalam list. input tabelNama untuk memanggil. sedangkan PrettyTable berfungsi untuk membungkus semua list. Deklarasi *a = 0* untuk membuat nomor pada isi table.
1. Membuat program perulangan menggunakan py while True:
1.  a += 1
 b = input("Masukkan Nama : ")
 c = input("Masukkan NIM : ")
 d = int(input("Masukkan Nilai Tugas : "))
 e = int(input("Masukkan Nilai UTS : "))
 f = int(input("Masukkan Nilai UAS :" ))
 g = "{:.2f}".format((d*.30) + (e*.35) + (f*.35))
a += 1 untuk menginput nomer pada awal table. deklarasi list dan Memasukkan Input Dengan Fungsi input() untuk menulis nama yang akan kita simpan dalam variabel. int(input()) untuk menginput tipe data interger (bilangan bulat) dalam variabel.

{:.2f}".format((d*.30) + (e*.35) + (f*.35)) untuk menginput Nilai Akhir yang di ambil dari perhitungan 3 komponen nilai.
1.  tabelNama.add_ro ([a,b,c,d,e,f,g])
 tabelNama.horizontal_char = "="
 tabelNama.junction_char = "="
 variabel di atas adalah untuk membentuk sebuah table.
1. Program input tanya [y/t], apabila jawaban t atau T, maka program inputan dihentikan statement break dan akan menampilkan data yang sudah diinput.

## Output
Bila dijalankan maka program akan menghasilkan output seperti dibawah ini :
<img width="960" alt="2" src="https://user-images.githubusercontent.com/115494491/203001750-5c7384a5-b728-448e-b952-b8fe622dd80e.png">