# <center>**Writing & Presentation Week 2**

## **Looping**<hr>
- ### **Deskripsi Loop**
  <div align="justify">
  Looping merupakan statement yang mengulang suatu instruksi hingga kondisi terpenuhi atau jika kondisi stop atau berhenti.<br>

  - Contoh macam Loop :
    - For Loop
    - While Loop
    - Do While Loop

  - Gambaran kapan kita harus menggunakan dari 3 macam Loop diatas.

    <img src="Gambar/loop.png">

- ### **For Loop**
  <div align="justify">
  digunakan jika kita tahu pasti seberapa banyak pengulangan yang ingin dilakukan pada program yang akan dikembangkan<br>
  contohnya :

  ```javascript
  for (let i = 1; i <= 10 ; i++) {
  console.log(i)
  }
  ```
- ### **While Loop**
  <div align="justify">
  While Loop akan menjalankan instruksi pengulangan bernilai TRUE Ada 2 macam while loop yaitu while dan do while<br>
  contoh perulangan while :

  ```javascript
  let i = 1 ; 
    while (i < 10){
        console.log(i);
        i ++ ;
    } 
  ```

- ### **Do While Loop**
  <div align="justify">

  ```javascript
  let i = 1;
  do {
    console.log(i);
    i++;
  } while (i <= 10);
  ```
- ### **Loop dengan Percabangan**

  ```javascript
    for (let i = 1; i <= 10 ; i++) {
    if (i == 6) {
      console.log(i , "yess ketemu")
    } else {
      console.log(i)
    }
  }
  ```
## **JavaScript Scope dan Function**<hr>
- ### **Scope**
  <div align="justify">
  adalah konsep dalam flow data variabel. Menentukan suatu variabel bisa diakses pada scope tertentu atau tidak.

- ### **Blocks**
  <div align="justify">
  Blocks adalah code yang berada didalam curly braces {}. Conditional, function, dan  looping menggunakan blocks.

- ### **Global Scope**
  <div align="justify">
  Global scope berarti variabel yang kita buat dapat diakses dimanapun dalam suatu file.Agar menjadi Global Scope, suatu variabel harus dideklarasikan diluar Blocks.<br>
  Contoh Global Scope :
 
  ```javascript
  let myName = "chaca" ; 
  function greeting()
     return myName;
  {
     console.log(myName);
  ```

- ### **Local Scope**
  <div align="justify">
  Local scope berarti kita mendeklarasikan variabel didalam blocks seperti function, conditional, dan looping.Maka variabel hanya bisa diakses didalam blocks saja. Tidak bisa diakses diluar blocks.<br>
  Contoh Local Scope :

    ```javascript
    function greetting(){
        let myName = "Arif";
        return myName;
    }
    console.log(gretting())
    console.log(myName);
    ```

- ### **Function**
    <div align="justify">Function adalah sebuah code blok dalam sebuah grup untuk menyelesaikan 1 task.<br>
    
    *Cara memanggil function :*
    ```javascript
    myFunction()
    console.log(myFunction());
    ```

    *Cara membuat function ada 3 :*
    - **Function Clasic**
        ```javascript
        function myFunction(kondisi) { }
        ```
    - **Function Variable**
        ```javascript
        let myFunction = function (kondisi) { }
        ```
    - **Arrow Function**
        ```
        let myFunction = (kondisi) => { }
        ```

- ### **Parameter Function**
    - <div align="justify">
      Dengan parameter, function dapat menerima sebuah inputan data dan menggunakannya untuk melakukan task/tugas.
    - <div align="justify">
      Saat membuat function/fitur, kita harus tahu data-data yang dibutuhkan. Misalnya saat membuat function penambahan 2 buah nilai. Data yang dibutuhkan adalah 2 buah nilai tersebut.

      ```javascript
      function penambahan (a,b){ // (a,b) merupakan parameter
          return a + b;
      }
      ```

- ### **Argumen Function**
    - <div align="justify">
      Argumen adalah nilai yang digunakan saat memanggil function.
    - <div align="justify">
      Jumlah argumen harus sama dengan jumlah parameternya

      ```javascript
      function penambahan (a,b){ // (a,b) merupakan parameter
          return a + b;
      }
      console.log(penambahan(5,5)) // (5,5) adalah argumen
      ```




