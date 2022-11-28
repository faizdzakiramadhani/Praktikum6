#Praktikum  6
#  Nama : Faiz Dzaki Ramadhani
#  Nim  : 31221O223
#  Kelas : TI.22.A2

#Tugas  6
<img width="585" alt="Screenshot_36" src="https://user-images.githubusercontent.com/115516635/204197503-e392016b-9a1e-4be6-bd68-701c167d33b0.png">


#Penjelasan  tugas 6


#  1.) Penggunaan if c.lower()
#  jika c.lower() fungsinya apabila user menginputkan denga huruf besar, maka otomatis akan menjadi huruf kecil sehingga kondisi yang digunakan tercapai. Contoh :
#  jika c.lower() == q
#  2.) Penggunaan while True
#  sedangkan True berfungsi untuk mendeteksi jika format yang diinputkan bukan berupa type maka akan muncul error
#  3.) Penggunaan lain
#  Fungsi else jika tidak error dan type yang dimasukan sesuai maka proses sedangkan True
#  4.) Penggunaan valueError
#  Fungsinya apabila diinputkan bukan berupa type maka hasilnya error (valueError)


#  Kode Program

``` Piton
daftarKontak = { " Nama " : " Nomer Telpon " }
kontak        = { ' Bayu ' : ' 081317611667 ' , ' Faiz ' : ' 0881024181723 ' , ' Dapit ' : ' 0877433331430 ' }
# cetak
cetak ( 30 * " ═ " )
print ( "     Nama | Nomor Telepon   " ) #prinr daftarkontak
cetak ( 30 * " - " )
print ( "    # Bayu | " , kontak[ ' Bayu ' ]) # print kontak Ayubi
print ( "    # Faiz | " , kontak[ ' Faiz ' ]) # print kontak Andi
print ( "    # Dapit | " , kontak[ ' Dapit ' ]) # print kontak Andi
cetak ( 30 * " ═ " )
#tampilkan kontaknya Ayubi
print ( " Tampilkan kontaknya Ayubi " )
print ( "     Bayu | " , kontak[ ' Bayu ' ]) # print kontak Ayubi
cetak ( 30 * " ═ " )
# kontak Tambah baru dengan nama Albed, nomor 081212273539
print ( " Tambah kontak baru dengan nama Albed, nomor 081212273539 " )
kontak[ ' Albed ' ] =  ' 081212273539 '
print ( "     Albed | " , kontak[ ' Albed ' ])
cetak ( 30 * " ═ " )
#Ubah kontak Andi dengan nomor baru 0876780147825
print ( " Ubah kontak Faiz dengan nomor baru 0881024181723 " )
kontak[ ' Faiz ' ] =  ' 0881024181723 '
print ( "     Faiz | " , kontak[ ' Faiz ' ])
cetak ( 30 * " ═ " )
# Tampilkan semua Nama
print ( " Tampilkan semua Nama " )
cetak (kontak.keys())
cetak ( 30 * " ═ " )
#Tampilkan semua Nomor
print ( " Tampilkan semua Nomor " )
cetak (kontak.values())
cetak ( 30 * " ═ " )
#tampilkan daftar Nama dan nomornya
print ( " Tampilkan daftar Nama dan nomornya " )
cetak (kontak.items())
cetak ( 30 * " ═ " )
# MengHapus kontak Andi
print ( " Hapus Kontak Dapit " )
kontak.pop( ' Dapit ' )
cetak (kontak.items())
cetak ( 30 * " ═ " )
```

#  Hasil Input Latihan 6
<img width="960" alt="Screenshot_35" src="https://user-images.githubusercontent.com/115516635/204196553-88ae9af7-34c9-4646-aefe-73e4b4dc99b6.png">

#Tugas  6
<img width="548" alt="Screenshot_37" src="https://user-images.githubusercontent.com/115516635/204197580-75d10461-961e-487e-8df2-b0a69f42ff9a.png">

``` Piton
mahasiswa = {}
def  menunjukkan ():
    jika mahasiswa.items():
        print ( " Daftar Nilai " )
        cetak ( " ============================================ ================================== " )
        print ( " | No | Nama | NIM | Tugas | UTS | UAS | Akhir | " )
        cetak ( " ============================================ ================================== " )
        saya =  0
        untuk mahasiswa.items ( ):
            saya +=  1
            print ( " | {no :2d } | {0 :14d } | {1 :11d } | {2 :7d } | {3 :7d } | {4 :7d } |       {5 :6.2f } | "
            .format (a[ 0 ][: 14 ],a[ 1 ][ 0 ],a[ 1 ][ 1 ],a[ 1 ][ 2 ],a[ 1 ][ 3 ],a[ 1 ][ 4 ], tidak ada  = i))
        cetak ( " ============================================ ================================== " )
        
    lain :
        print ( " Daftar Nilai " )
        cetak ( " ============================================ ================================== " )
        print ( " | No | Nama | NIM | Tugas | UTS | UAS | Akhir | " )
        cetak ( " ============================================ ================================== " )
        print ( " | TIDAK ADA DATA | " )
        cetak ( " ============================================ ================================== " )
pasti  tambahkan ():
    print ( " Tambah Data " )
    nama =  input ( " Nama \t : " )
    nim =  input ( " NIM \t : " )
    uts =  int ( input ( " Nilai UTS \t : " ))
    uas =  int ( input ( " Nilai UAS \t : " ))
    tugas =  int ( input ( " Nilai Tugas \t : " ))
    akhir = (tugas *  30 / 100 ) + (uts *  35 / 100 ) + (uas *  35 / 100 )
    mahasiswa[nama] = nim, tugas, uts, uas, akhir
pasti  hapus ():
    print ( " Hapus Data " )
    nama =  input ( " Masukkan Nama : " )
    
    jika nama di mahasiswa.keys():
        del mahasiswa[nama]
    
    lain :
        print ( " Nama tidak ditemukan " )
def  pembaruan ():
    print ( " Ubah Data " )
    nama =  input ( " Masukkan Nama : " )
    jika nama di mahasiswa.keys():
        nim =  input ( " NIM \t : " )
        uts =  int ( input ( " Nilai UTS \t : " ))
        uas =  int ( input ( " Nilai UAS \t : " ))
        tugas =  int ( input ( " Nilai Tugas \t : " ))
        akhir = (tugas *  30 / 100 ) + (uts *  35 / 100 ) + (uas *  35 / 100 )
        mahasiswa[nama] = nim, tugas, uts, uas, akhir
    lain :
        print ( " Nama tidak ditemukan " )
 pencarian def ():
    print ( " Cari Data " )
    a =  input ( " Masukkan Nama : " )
    jika a dalam mahasiswa.keys():
        cetak ( " ============================================ ============================ " )
        print ( " | Nama | NIM | Tugas | UTS | UAS | Akhir | " )
        cetak ( " ============================================ ============================ " )
        cetak ( " | {0 :14d } | {1 :11d } | {2 :7d } | {3 :7d } | {4 :7d } |      {5 :6.2f } | "
            .format (a , mahasiswa[a][ 0 ], mahasiswa[a][ 1 ], mahasiswa[a][ 2 ], mahasiswa[a][ 3 ], mahasiswa[a][ 4 ] ))
        cetak ( " ============================================ ============================ " )
    lain :
        cetak ( " ============================================ ================================== " )
        print ( " | No | Nama | NIM | Tugas | UTS | UAS | Akhir | " )
        cetak ( " ============================================ ================================== " )
        print ( " | DATA TIDAK DITEMUKAN | " )
        cetak ( " ============================================ ================================== " )
 menu def ():
    cetak ( " \n " )
    cetak ( " ================================ " )
    print ( "       Nilai Masukan Program        " )
    cetak ( " ================================ \n " )
    x =  input ( " [(L)ihat, (T)ambah, (U)bah, (H)apus, (C)ari, (K)eluar]: " )
    cetak ( " \n " )
    jika x ==  ' L ' :
        menunjukkan()
    elif x ==  ' T ' :
        menambahkan()
    elif x ==  ' U ' :
        memperbarui()
    elif x ==  ' H ' :
        menghapus()
    elif x ==  ' C ' :
        Cari()
    elif x ==  ' K ' :
        cetak ( " ============================================ =========================== " )
        cetak ( ' \n ' )
        print ( " > Anda keluar dari kode                         " )
        cetak ( " \n " )
        cetak ( " ============================================ =========================== " )
        keluar ()
    lain :
        print ( "             KODE YANG ANDA MASUKKAN TIDAK VALID !!!!!!!!!!! " )
sementara  Benar :
    Tidak bisa()
```
#  Hasil Masukan
<img width="960" alt="1" src="https://user-images.githubusercontent.com/115516635/204199085-80499ca1-61ea-46c1-9ca9-b15adeee9327.png">

#  Flowchart

![ pppp ](https://user-images.githubusercontent.com/115516730/204177502-8a430533-143f-4748-801d-0c4380e12328.png)

