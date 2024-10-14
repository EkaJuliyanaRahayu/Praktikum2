# Praktikum2

<p>Buatlah kode program java untuk:</p>
<p>• Mendeklarasikan class Person, dengan
atribut Nama, JenisKelamin, Umur dan
lengkapi dengan access modifier.</p>
<p>• Buatlah dua buah objek dari class Person
bernama Anton dan Riko dan panggil
method setter dan getter.</p>

![Screenshot 2024-10-14 074427](https://github.com/user-attachments/assets/59ff1e33-2686-456f-a42d-500d8aebd14c)

# - Mendeklarasikan class person dengan dilengkapi access modifier

## *Access Modifier `private` pada atribut nama, jenis kelamin, umur
```
// Deklarasi atribut
    private String nama;
    private String jenisKelamin;
    private int umur;
```
<p>• Atribut nama, jenisKelamin, dan umur menggunakan access modifier ` private `. Berarti 
  atribut tersebut hanya dapat di akses oleh kelas itu saja yaitu class person</p>

## *Access Modifier `public` pada `class Person`, `constructor Person`, semua `getter` dan `setter`, method `tampilkanInfo`, dan `method main`
```
public class Person {
```
```
// Constructor untuk menginisialisasi atribut
    public Person(String nama, String jenisKelamin, int umur) {
        this.nama = nama;
        this.jenisKelamin = jenisKelamin;
        this.umur = umur;
    }

    // Getter dan Setter untuk atribut nama
    public String getNama() {
        return nama;
    }

    public void setNama(String nama) {
        this.nama = nama;
    }

    // Getter dan Setter untuk atribut jenisKelamin
    public String getJenisKelamin() {
        return jenisKelamin;
    }

    public void setJenisKelamin(String jenisKelamin) {
        this.jenisKelamin = jenisKelamin;
    }

    // Getter dan Setter untuk atribut umur
    public int getUmur() {
        return umur;
    }

    public void setUmur(int umur) {
        this.umur = umur;
    }

    // Method untuk menampilkan informasi tentang person
    public void tampilkanInfo() {
        System.out.println("Nama: " + nama);
        System.out.println("Jenis Kelamin: " + jenisKelamin);
        System.out.println("Umur: " + umur);
    }
    
    public static void main(String[] args) {
        // Membuat objek Person bernama Antor dan Riko
        Person antor = new Person("Anton", "Laki-laki", 25);
        Person riko = new Person("Riko", "Laki-laki", 35);
```
<p>• class Person, constructor Person, semua getter dan setter, method tampilkanInfo, dan method main menggunakan access modifier `public`. 
mereka menggunakan access modifier `public`, berarti mereka dapat dipanggil diluar kelas `person`</p>

# - Membuat dua buah objek dengan memanggil metode getter dan setter</p>

## * Membuat dua buah objek `Anton` dan `Riko`
```
 // Membuat objek Person bernama Antor dan Riko
        Person antor = new Person("Anton", "Laki-laki", 25);
        Person riko = new Person("Riko", "Laki-laki", 35);
```
## * Memangil metode `Getter` dan `Setter`</p>
# `Getter` dan `Setter` untuk nama
```
 // Getter dan Setter untuk atribut nama
    public String getNama() {
        return nama;
    }

    public void setNama(String nama) {
        this.nama = nama;
    }
```
# `Getter` dan `Setter` untuk jenis kelamin
```
 // Getter dan Setter untuk atribut jenisKelamin
    public String getJenisKelamin() {
        return jenisKelamin;
    }

    public void setJenisKelamin(String jenisKelamin) {
        this.jenisKelamin = jenisKelamin;
    }
```
# `Getter` dan `Setter` untuk umur
```
 // Getter dan Setter untuk atribut umur
    public int getUmur() {
        return umur;
    }

    public void setUmur(int umur) {
        this.umur = umur;
    }
```
<p>• Method getter untuk (getNama, getJenisKelamin, getUmur) digunakan untuk mendapatkan informasi dari masing-masing objek (Anton dan Riko) dan menampilkannya.</p>
<p>• Method setter (setNama, setUmur) digunakan untuk mengubah nilai atribut nama dan umur dari objek (Anton dan Riko).</p>
<p>• Setelah perubahan melalui setter, maka informasi baru dari kedua objek ditampilkan menggunakan getter.</p>

## INPUT
```

package person;

public class Person {
    // Deklarasi atribut
    private String nama;
    private String jenisKelamin;
    private int umur;

    // Constructor untuk menginisialisasi atribut
    public Person(String nama, String jenisKelamin, int umur) {
        this.nama = nama;
        this.jenisKelamin = jenisKelamin;
        this.umur = umur;
    }

    // Getter dan Setter untuk atribut nama
    public String getNama() {
        return nama;
    }

    public void setNama(String nama) {
        this.nama = nama;
    }

    // Getter dan Setter untuk atribut jenisKelamin
    public String getJenisKelamin() {
        return jenisKelamin;
    }

    public void setJenisKelamin(String jenisKelamin) {
        this.jenisKelamin = jenisKelamin;
    }

    // Getter dan Setter untuk atribut umur
    public int getUmur() {
        return umur;
    }

    public void setUmur(int umur) {
        this.umur = umur;
    }

    // Method untuk menampilkan informasi tentang person
    public void tampilkanInfo() {
        System.out.println("Nama: " + nama);
        System.out.println("Jenis Kelamin: " + jenisKelamin);
        System.out.println("Umur: " + umur);
    }
    
    public static void main(String[] args) {
        // Membuat objek Person bernama Antor dan Riko
        Person antor = new Person("Anton", "Laki-laki", 25);
        Person riko = new Person("Riko", "Laki-laki", 35);

        // Menampilkan informasi untuk Antor
        System.out.println("Informasi Anton:");
        antor.tampilkanInfo();

        // Menampilkan informasi untuk Riko
        System.out.println("\nInformasi Riko:");
        riko.tampilkanInfo();
    }
}
    
   ```

## OUTPUT
![Screenshot 2024-10-14 083427](https://github.com/user-attachments/assets/4cbbff6c-0af3-4068-8af2-982187a08ad2)


