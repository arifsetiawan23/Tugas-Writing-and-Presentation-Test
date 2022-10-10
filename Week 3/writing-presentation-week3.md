# <center>**Writing & Presentation Week 3**

## **Array dan Multidimensional Array**<hr>
- ### **Array**
  - **Array** merupakan pengorganisasian data dan tempat penyimpanan data
  - **Array** adalah tipe data list order yang dapat menyimpan tipe data apapun dialamnya seperti string, number, boolean dan lainnya<br>
  contoh Array

    ```javascript
    let nama = ["Arif", 22, true ];
    ```
- ### **Memanggil Array**
  <div align="justify">
  Array pada javascript dihitung dari index data ke-0.
  Data pertama adalah index ke-0.
  
  ```javascript
  console.log(nama); //memanggil semua data
  console.log(nama[0]); //memanggil data index ke 0
  console.log(nama[1]); // memanggil data index ke 1
  console.log(nama[2]); //memanggil data index ke 2
  console.log(arr.length); //panjang data array

- ### **Update Array**
  <div align="justify">
  Seperti tipe data dan variabel pada umumnya, kita dapat mengupdate data pada Array

  ```javascript
  let nama = ["Arif", 22, true ];
  nama[0] = "Arif Setiawan"

  console.log(nama)
  // output : ["Arif Setiawan", 1 , true]
  ```
- ### **Array Method**
  <div align="justify">
  Array memiliki method atau biasa disebut built-in methods, yang sama dengan function yang dapat digunakan kapan saja kita membutuhkannya.

  - **push** menambahkan array pada index terakhir
    ```javascript
    let arrHp = ["xiomy", "oppo", "samsung", "realme","iphone"]
    arrHp.push("infinix");
    
    console.log(mobil)
    // Output : ["xiomy", "oppo", "samsung", "realme","iphone", "infinix"]
    ```
  
  - **pop** Menghapus array pada index terakhir
    ```javascript
    let arrHp = ["xiomy", "oppo", "samsung", "realme","iphone"]
    arrHp.pop();
    
    console.log(mobil)
    // Output : ["xiomy", "oppo", "samsung", "realme"]
    ```
  - **shift** Menghapus array pada index pertama
    ```javascript
    let arrHp = ["xiomy", "oppo", "samsung", "realme","iphone"]
    arrHp.shift()
    console.log(arrHp)
    // Output : ["oppo", "samsung", "realme", "iphone"]

  - **unshif** Menambahkan array pada index pertama

    ```javascript
    let arrHp = ["xiomy", "oppo", "samsung", "realme","iphone"]
    arrHp.unshift('pocophone')

    console.log(mobil)
    // Output : ["pocophone", "xiomy", "oppo", "samsung", "realme"]
    ```
  - **sort** Mengurutkan array secara ascending maupun descending
    
    let angka = [1, 3, 4, 2]
    angka.sort()
    console.log(angka)
    // Output : [1, 2, 3, 4]
  
    


  