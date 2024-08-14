# Proyek Akhir Pemrograman Berbasis Objek 1

Proyek ini adalah contoh sederhana aplikasi pengolahan data mahasiswa menggunakan Java sebagai tugas akhir dari mata kuliah pemrograman berbasis objek 1.

## Deskripsi

Aplikasi ini menerima input berupa nama dan NPM mahasiswa, dan memberikan output berupa informasi detail dari NPM tersebut seperti tahun masuk, fakultas, program studi, dan nomor registrasi.

Aplikasi ini mengimplementasikan beberapa konsep penting dalam pemrograman berorientasi objek (OOP) seperti Class, Object, Atribut, Method Constructor, Method Mutator, Method Accessor, Encapsulation, Inheritance, Overloading, Overriding, Seleksi, Perulangan, IO Sederhana, Array, dan Error Handling.

## Penjelasan Kode

Berikut adalah bagian kode yang relevan dengan konsep OOP yang dijelaskan:

1. **Class** adalah template atau blueprint dari object. Pada kode ini, `Karyawan`, `PegawaiKontrak`, dan `PegawaiTetap` adalah contoh dari class.

```bash
public class Karyawan {
    ...
}

public class PegawaiKontrak extends Karyawan {
    ...
}

public class PegawaiTetap extends Karyawan {
    ...
}
```

2. **Object** adalah instance dari class. Pada kode ini, `mhs[i] = new PegawaiKontrak(nama, id);` adalah contoh pembuatan object.

```bash
mhs[i] = new MahasiswaDetail(nama, npm);
```

3. **Atribut** adalah variabel yang ada dalam class. Pada kode ini, `nama` dan `id` adalah contoh atribut.

```bash
String nama;
String id;
```

4. **Constructor** adalah method yang pertama kali dijalankan pada saat pembuatan object. Pada kode ini, constructor ada di dalam class `Karyawan` dan `PegawaiKontrak`.

```bash
public Karyawan (String nama, String id) {
    this.nama = nama;
    this.id = id;
}

public PegawaiKontrak(String nama, String id) {
    super(nama, id);
}
```

5. **Mutator** atau setter digunakan untuk mengubah nilai dari suatu atribut. Pada kode ini, `setNama` dan `setId` adalah contoh method mutator.

```bash
public void setNama(String nama) {
    this.nama = nama;
}

public void setId(String Id) {
    this.Id = Id;
}
```

6. **Accessor** atau getter digunakan untuk mengambil nilai dari suatu atribut. Pada kode ini, `getNama`, `getId`, `getUpahPerJam`, `getJumlahJamKerja`, `getGajiPokok` adalah contoh method accessor.

```bash
public String getNama() {
    return nama;
}

public String getId() {
    return Id;
}
```

7. **Encapsulation** adalah konsep menyembunyikan data dengan membuat atribut menjadi private dan hanya bisa diakses melalui method. Pada kode ini, atribut `nama` dan `Id` dienkapsulasi dan hanya bisa diakses melalui method getter dan setter.

```bash
private String nama;
private String Id;
```

8. **Inheritance** adalah konsep di mana sebuah class bisa mewarisi property dan method dari class lain. Pada kode ini, `PegawaiKontrak` mewarisi `Karyawan` dengan sintaks `extends`.

```bash
public class PegawaiKontrak extends Karyawan {
    ...
}
```

9. **Polymorphism** adalah konsep di mana sebuah nama dapat digunakan untuk merujuk ke beberapa tipe atau bentuk objek berbeda. Ini memungkinkan metode-metode dengan nama yang sama untuk berperilaku berbeda tergantung pada tipe objek yang mereka manipulasi, polymorphism bisa berbentuk Overloading ataupun Overriding. Pada kode ini, method `displayInfo(String)` di `Mahasiswa` merupakan overloading method `displayInfo` dan `displayInfo` di `MahasiswaDetail` merupakan override dari method `displayInfo` di `Mahasiswa`.

```bash
public String getInfo() {
        return super.getInfo() + "\nUpah Per Jam: " + getUpahPerJam() + "\nJumlah Jam Kerja: " + getJumlahJamKerja();
}

@Override
public String displayInfo() {
    ...
}
```

10. **Seleksi** adalah statement kontrol yang digunakan untuk membuat keputusan berdasarkan kondisi. Pada kode ini, digunakan seleksi `if else` dalam method `getFakultas` dan seleksi `switch` dalam method `getProdi`.

```bash
pu switch (opsi) {
                case 1:
                    for (Karyawan karyawan : karyawans) {
                        System.out.println(karyawan.getNama() + " - " + karyawan.getId());
                    }
                    break;
}

pucase 2:
                    for (Karyawan karyawan : karyawans) {
                        System.out.println(karyawan.getInfo());
                        System.out.println("Gaji: " + karyawan.hitungGaji());
                        System.out.println("---------------------------");
                    }
                    break;
    }
}
```

11. **Perulangan** adalah statement kontrol yang digunakan untuk menjalankan blok kode berulang kali. Pada kode ini, digunakan loop `for` untuk meminta input dan menampilkan data.

```bash
for (int i = 0; i < mahasiswas.length; i++) {
    ...
}
```

12. **Input Output Sederhana** digunakan untuk menerima input dari user dan menampilkan output ke user. Pada kode ini, digunakan class `Scanner` untuk menerima input dan method `System.out.println` untuk menampilkan output.

```bash
Scanner scanner = new Scanner(System.in);
System.out.print("Masukkan Nama Mahasiswa ke-" + (i + 1) + ": ");
String nama = scanner.nextLine();

System.out.println("\nData Mahasiswa:");
System.out.println(mahasiswa.displayInfo());
```

13. **Array** adalah struktur data yang digunakan untuk menyimpan beberapa nilai dalam satu variabel. Pada kode ini, `MahasiswaDetail[] mahasiswas = new MahasiswaDetail[2];` adalah contoh penggunaan array.

```bash
MahasiswaDetail[] mahasiswas = new MahasiswaDetail[2];
```

14. **Error Handling** digunakan untuk menangani error yang mungkin terjadi saat runtime. Pada kode ini, digunakan `try catch` untuk menangani error.

```bash
try {
    // code that might throw an exception
} catch (Exception e) {
    System.out.println("Error: " + e.getMessage());
}
```

## Usulan nilai

| No  | Materi         |  Nilai  |
| :-: | -------------- | :-----: |
|  1  | Class          |    5    |
|  2  | Object         |    5    |
|  3  | Atribut        |    5    |
|  4  | Constructor    |    5    |
|  5  | Mutator        |    5    |
|  6  | Accessor       |    5    |
|  7  | Encapsulation  |    5    |
|  8  | Inheritance    |    5    |
|  9  | Polymorphism   |   10    |
| 10  | Seleksi        |    5    |
| 11  | Perulangan     |    5    |
| 12  | IO Sederhana   |   10    |
| 13  | Array          |   15    |
| 14  | Error Handling |   15    |
|     | **TOTAL**      | **100** |

## Pembuat

Nama: Riski Maulana Prayoga
NPM: 2210010715
