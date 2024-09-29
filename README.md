#include <stdio.h>
#include <conio.h>



class Karyawan:
    char __ init __ (self, nama, gaji):
       lf.nama = nama
        self.gaji = gaji
        self.potongan = 0

    def hitung_gaji_bersih(self):
        return self.gaji - self.potongan

def tambah_karyawan():
    nama = input("Masukkan nama karyawan: ")
    gaji = float(input("Masukkan gaji karyawan: "))
    karyawan_baru = Karyawan(nama, gaji)
    karyawan.append(karyawan_baru)

def tampilkan_karyawan():
    for karyawan in karyawan:
        print(f"Nama: {karyawan.nama}, Gaji: {karyawan.gaji}, Gaji Bersih: {karyawan.hitung_gaji_bersih()}")

def main():
    karyawan = []
    while True:
        print("1. Tambahkan data karyawan")
        print("2. Tampilkan data karyawan")
        print("3. Keluar")
         pilihan = input("Masukkan pilihan: ")
        if pilihan == "1":
            tambah_karyawan()
        elif pilihan == "2":
            tampilkan_karyawan()
        elif pilihan == "3":
            break
        else:
            print("Pilihan tidak valid")

if _name_ == "_main_":
    main()
