# Latihan Praktikum 5

## Hasil Latihan Praktikum 5 
````Python
data_mahasiswa = []

while True:
    print("="*23)
    print("Masukkan Data Mahasiswa")
    print("="*23)
    nama = input("Nama: ")
    nim = input("NIM: ")
    tugas = float(input("Nilai Tugas: "))
    uts = float(input("Nilai UTS: "))
    uas = float(input("Nilai UAS: "))

    nilai_akhir = (tugas * 0.3) + (uts * 0.35) + (uas * 0.35)

    data_mahasiswa.append({
        "nama": nama,
        "nim": nim,
        "tugas": tugas,
        "uts": uts,
        "uas": uas,
        "nilai_akhir": nilai_akhir
    })

    tambah_data = input("Tambah Data(y/t)? ")
    if tambah_data == 't':
        break

# Lebar kolom untuk setiap data
print("=" * 95)
print(f"{'No'.center(5)}|{'Nama'.center(15)}|{'NIM'.center(10)}|{'Nilai Tugas'.center(13)}|{'Nilai UTS'.center(10)}|{'Nilai UAS'.center(10)}|{'Nilai Akhir'.center(10)}")
print("=" * 95)

for i, mhs in enumerate(data_mahasiswa, start=1):
    print(f"{str(i).center(5)}|{mhs['nama'].center(15)}|{mhs['nim'].center(10)}|{str(mhs['tugas']).center(13)}|{str(mhs['uts']).center(10)}|{str(mhs['uas']).center(10)}|{format(mhs['nilai_akhir'], '.2f').center(10)}")

````

## Hasil Output Praktikum 5

```markdown
=======================
Masukkan Data Mahasiswa
=======================
Nama: ALDI 
NIM: 3124
Nilai Tugas: 99
Nilai UTS: 89
Nilai UAS: 99
Tambah Data(y/t)? y
=======================
Masukkan Data Mahasiswa
=======================
Nama: AGUS
NIM: 3124
Nilai Tugas: 90
Nilai UTS: 89
Nilai UAS: 99
Tambah Data(y/t)? t
===============================================================================================
  No |      Nama     |   NIM    | Nilai Tugas |Nilai UTS |Nilai UAS |Nilai Akhir
===============================================================================================
  1  |     ALDI      |   3124   |     99.0    |   89.0   |   99.0   |  95.50
  2  |      AGUS     |   3124   |     90.0    |   89.0   |   99.0   |  92.80
```
# Penjelasan Latihan Praktikum 5
