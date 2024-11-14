# Latihan Praktikum 5

## Hasil Latihan Praktikum 5 
````Python
data_mahasiswa = []

while True:
    print("\nMasukkan data mahasiswa:")
    nama = input("Nama: ")
    nim = input("NIM: ")
    tugas = float(input("Nilai Tugas: "))
    uts = float(input("Nilai UTS: "))
    uas = float(input("Nilai UAS: "))

    nilai_akhir = (tugas * 0.3) + (uts * 0.35) + (uas * 0.35)

    data_mahasiswa.append({
        'nama': nama,
        'nim': nim,
        'tugas': tugas,
        'uts': uts,
        'uas': uas,
        'nilai_akhir': nilai_akhir
    })

    tambah = input("\nTambah data lagi? (y/t): ").lower()
    if tambah == 't':
        break

print("\nDaftar Nilai Mahasiswa:")
print("="*80)
print(f"{'Nama':<15} {'NIM':<10} {'Tugas':<10} {'UTS':<10} {'UAS':<10} {'Nilai Akhir':<10}")
print("="*80)

for mhs in data_mahasiswa:
    print(f"{mhs['nama']:<15} {mhs['nim']:<10} {mhs['tugas']:<10} {mhs['uts']:<10} {mhs['uas']:<10} {mhs['nilai_akhir']:<10.2f}")

print("="*80)
````

## Hasil Output Praktikum 5

```markdown
Masukkan data mahasiswa:
Nama: ALDI RISMANDAYANA
NIM: 312410015
Nilai Tugas: 99
Nilai UTS: 89
Nilai UAS: 99

Tambah data lagi? (y/t): t

Daftar Nilai Mahasiswa:
================================================================================
Nama            NIM        Tugas      UTS        UAS        Nilai Akhir
================================================================================
ALDI RISMANDAYANA 312410015  99.0       89.0       99.0       95.50
================================================================================
```
# Penjelasan Latihan Praktikum 5
