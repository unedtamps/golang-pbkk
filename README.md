# Tutorial Golang PBKK D

- Nama : Unedo Viery Kristenzky Tampubolon
- NRP : 5025221116

# Penjelasan

Penjelasan mengenai kode program yang ada pada repository ini adalah sebagai berikut:

1. Variables
    
    Variabel dalam bahasa pemrograman Go dideklarasikan dengan cara berikut:
    ```go
    var namaVariabel tipeData = nilai
    ```

    Contoh:
    ```go
    var nama string = "Unedo"
    ```

    Variabel juga bisa dideklarasikan tanpa menyebutkan tipe datanya, Go akan secara otomatis menentukan tipe data dari nilai yang diberikan:
    ```go
    nama := "Unedo"
    ```
   

2. Array

    Array dalam bahasa pemrograman Go adalah kumpulan elemen yang memiliki tipe data yang sama. Array memiliki ukuran yang tetap dan tidak bisa diubah setelah dideklarasikan. Array dalam Go dideklarasikan dengan cara berikut:
    ```go
    arr := [5]int{1, 2, 3, 4, 5}
    ```

3. Slice

    Slice dalam bahasa pemrograman Go adalah potongan dari array. Slice memiliki ukuran yang dinamis, berbeda dengan array yang memiliki ukuran tetap. Slice dalam Go dideklarasikan dengan cara berikut:
    ```go
    slice := []int{1, 2, 3, 4, 5}
    ```

4. Looping

    Go memiliki satu jenis perulangan yaitu `for`. Perulangan `for` dalam Go memiliki tiga bentuk, yaitu:
    - `for` dengan satu kondisi
    - `for` dengan tiga kondisi
    - `for` seperti `while`

    Contoh:
    ```go
    for i := 0; i < 5; i++ {
        fmt.Println(i)
    }
    ```
    Atau dapat juga loop menggunakan `range`:
    ```go
    arr := []int{1, 2, 3, 4, 5}
    for index, value := range arr {
        fmt.Println(index, value)
    }
    ```

5. If-Else

    Go memiliki struktur percabangan `if-else` yang
    digunakan untuk mengeksekusi blok kode tertentu jika kondisi yang diberikan bernilai benar. Contoh:
    ```go
    if x > 5 {
        fmt.Println("x lebih besar dari 5")
    } else {
        fmt.Println("x kurang dari atau sama dengan 5")
    }
    ```

6. Function
    
    Fungsi dalam bahasa pemrograman Go dideklarasikan dengan cara berikut:
    ```go
    func namaFungsi(parameter tipeData) tipeData {
        // kode program
    }
    ```

    Contoh:
    ```go
    func tambah(a int, b int) int {
        return a + b
    }
    ```

    Fungsi juga bisa mengembalikan lebih dari satu nilai:
    ```go
    func tambahKurang(a int, b int) (int, int) {
        return a + b, a - b
    }
    ```

7. Maps

    Maps dalam bahasa pemrograman Go adalah kumpulan pasangan key-value. Maps dalam Go dideklarasikan dengan cara berikut:
    ```go
    m := map[string]int{
        "foo": 1,
        "bar": 2,
    }
    ```
    Untuk mengakses nilai dari maps, kita bisa menggunakan key-nya:
    ```go
    fmt.Println(m["foo"])
    ```

8. Struct

   Struct dalam bahasa pemrograman Go adalah kumpulan dari beberapa field. Struct dalam Go dideklarasikan dengan cara berikut:
   ```go
    type Person struct {
         Name string
         Age  int
    }
    ```
    Untuk mengakses field dari struct, kita bisa menggunakan `.`:
    ```go
    p := Person{Name: "Unedo", Age: 20}
    fmt.Println(p.Name)
    ```

9. Scope Rules

   Dalah bahasa pemrograman Go, variabel yang dideklarasikan di luar fungsi bersifat global dan bisa diakses dari seluruh bagian program. Sedangkan variabel yang dideklarasikan di dalam fungsi bersifat lokal dan hanya bisa diakses dari dalam fungsi tersebut. 
