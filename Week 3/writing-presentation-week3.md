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
    
    console.log(arrHp)
    // Output : ["xiomy", "oppo", "samsung", "realme","iphone", "infinix"]
    ```
  
  - **pop** Menghapus array pada index terakhir
    ```javascript
    let arrHp = ["xiomy", "oppo", "samsung", "realme","iphone"]
    arrHp.pop();
    
    console.log(arrHp)
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
    arrHp.unshift ('pocophone')

    console.log(arrHp)
    // Output : ["pocophone", "xiomy", "oppo", "samsung", "realme"]
    ```
  - **sort** Mengurutkan array secara ascending maupun descending
    ```javascript
    let angka = [1, 3, 4, 2]
    angka.sort()
    console.log(angka)
    // Output : [1, 2, 3, 4]
    ```

- ### **Looping pada Array**
    - Array memiliki built in methods untuk melakukan looping yaitu .map() dan .forEach()
        - **forEach** method untuk melakukan looping pada setiap elemen array.

            ```javascript
            let arrHp = ["xiomy", "oppo", "samsung", "realme","iphone"]
            arrHp.forEach(elemnt => {
            console.log(element); 
            })
            ```
        - **map** melakukan perulangan/looping dengan membuat array baru.

             ```javascript
             let angka = [1, 3, 4, 2]
             let double = angka.map(num =>{
                return num * 2
             })

             console.log(double)
             // Output : [2, 6, 8, 4]
             ```
- ### **Array Multidimensi** 
   <div align="justify">
   Adalah array didalam array atau bisa dianalogikan dengan array of array. <br>
   Struktur Array Multidimensional :

   ```javascript
       let nama =[
            ["arif", 22, true ],
            ["setiawan", 20, false ],
    ];
    ```

## **JavaScript Object & Array of Object** <hr>
- ### **Object**
  object adalah sebuah tipe data pada variabel yang menyimpan properti dan fungsi (method)

  - **Membuat sebuah object**
    - Sama seperti tipe data sebelumnya. Object dapat diassign kedalam sebuah variabel.
    - object person dengan properti
      ```javascript
      let person = {
        name : 'Arif',
        age : 20,
        isVarified : true
      }
      ```

- ### **Mengakses Object dan Property Object**
    - **akses seluruh object**
        ```javascript
        let person = {
            name : 'Arif',
            age : 22,
            isVarified : true
        }
        console.log(person)
        ```
    - **Mengakses properti object**
        ```javascript
        let person = {
            name : 'Arif',
            age : 22,
            isVarified : true
        }
        console.log(person.name) // 'Arif'
        ```

    - **Bracket Notation**
       <div align="justify">Kita juga bisa menggunakan bracket notation saat memanggil properti dari sebuah object.

        ```javascript
        let person = {
            name : 'Arif',
            age : 22,
            isVarified : true
        }
        console.log(person['name']) // 'Arif'
        console.log(person['age']) // 22
        ```
- ### **Update Object**
  <div align="justify">
  Kita dapat melakukan update pada variabel dengan tipe data Object.
    
  - **Update data pada Object**
    ```javascript
    let person = {
        name : 'Arif',
        age : 22,
        isVarified : true
    }
    person.age = 23;
    person,addres = 'Ngawi, Paron';

    console.log(person)
    /* Output :
    {
        name : 'Arif',
        age : 23,
        isVarified : true
        addres : 'Ngawi, Paron'
    } */
    ```

- ### **Delete Object Property**
    - Kita dapat menghapus properti dari object menggunakan delete operator.
        ```javascript
            const person = {
                name : 'Arif',
                age : 22,
                isVarified : true
            }
            delete person.age;
            console.log(person) 
            /* Output :
            {
                name : 'Arif',
                isVarified : true
            }

        ```
- ### **Method**
    - Jika value yang kita masukkan pada property berupa function.Maka itu disebut Method.
    - Kita bisa membuat method custom untuk kita gunakan pada aplikasi kita.
    - Ada 2 method pada object greeting
        ```javascript
        const greeting = {
            welcome : function () {
                return 'Hallo selamat datang';
            },
            afterTransaction : function () {
                return "terima kasih sudah membeli produk kami";
            },
        };

        console.log(greeting.welcome()); // Hallo selamat datang
        ```

- ### **Nested Object**
    - Pada real application nanti kalian pasti menemukan data object yang kompleks. Object yang berasal dari turunan object lainnya.
    - Contoh : Data article pada sebuah aplikasi berita
        ```javascript
        const news = {
            title: 'Impact Byte menjadi Unicorn',
            description: 'lorem ipsunm jkkrj kekek kejkje jjejhej ',
            author : {
                people : {
                    name : 'Arif',
                    age : 22,
                    city : 'Ngawi'
                }
            }
        };
        console.log('news:', news.title);
        console.log('Article publised by', news.author.people.news);
        ```

- ### **Looping Object**
    - Jika kita ingin menampilkan seluruh object properti. Kita bisa menggunakan looping.
        ```javascript
        for(let key in object){
            //..
        }
        ```
- ### **Array of Object**
    - **Looping pada Data array of object**

        ```javascript
        let students = [
            {
                name : "Arif",
                age : 22,
                isVarified : true
            },
            {
                name : "Setiawan",
                age : 22,
                isVarified : false
            },
        ];

        // gunakan forEach jika object dalam array
        students.forEach((ListStudent) => {
            console.log(ListStudent)
        })
        ```

## **JavaScript Rekursif** <hr>
- ### **Deskripsi Recursif**
  <div align="justify">
  Recursive adalah function yang memanggil dirinya sendiri sampai kondisi tertentu. Recursive kebanyakan digunakan untuk case matematika.<br>
  Contoh :

    ```javascript
    function reqursive(){
        // ..
        reqursive();
        // ..
    }
    ```

    ```javascript
    function reqursive(){
        if (conditional){
            //..
        }else{
            reqursive();
        }
    };
    ```


- ### **Ciri dari rekursif**
  - <div align="justify">Fungsi rekursif selalu memiliki kondisi yang menyatakan kapan fungsi tersebut berhenti. Kondisi ini harus dapat dibuktikan akan tercapai, karena jika tidak tercapai maka kita tidak dapat membuktikan bahwa fungsi akan berhenti, yang berarti algoritma kita tidak benar.

  - <div align="justify">Fungsi rekursif selalu memanggil dirinya sendiri sambil mengurangi atau memecahkan data masukan setiap panggilannya. Hal ini penting diingat, karena tujuan utama dari rekursif ialah memecahkan masalah dengan mengurangi masalah tersebut menjadi masalah-masalah kecil.

- ### **Contoh kasus rekursif**
    - Fungsi rekursif menghitung mundur number
        ```javascript
        function countDown(fromNumber) {
            console.log(fromNumber)
            let nextNumber = fromNumber - 1;

            if (nextNumber > 0) {
            countDown(nextNumber);
            }
        }
        countDown(3);
        // Output : 
        3
        2
        1 //
        ```

## **JavaScript Modules**<hr>

- ### **Deskripsi JS Modules**
  Js Modules adalah cara untuk memisahkan kode file yang berbeda
  - Keuntungan menggunakan modules : 
    - mudah untuk mengelola file
    - kode tidak menumpuk pada satu file

- ### **Membuat Js Modules**
    - tambahkan type= `"module"` pada script utama
        ```javascript
        <script src="indonesia.js" type="module"></script>
        ```
    - siapkan script ke-2 dan seterusnya untuk melakukan export
    - lakukan import pada file/script utama

- ### **Contoh Export Import js module**
    - script `Amerika.js`
        ```javascript
        let apple = ["iphone", "macbook", "imac"]
        export {apple}
        ```
    - script `jepang.js`
        ```javascript
        import {apple} from './amerika.js';
        console.log(apple);

        let motor = ["suzuki", "yamaha", "honda", "kawasaki"]
        const smartPhone = ["sony", "samsung", "fujitsu", "LG"]

        let dokumenNegara = "Hello"

        export function sayHello() {
        console.log("hallooo")
        }
        let entertainment = ["anime", "manga", "wibu", "dorama"]

        // kita dapat melakukan export pada variabel, function, class
        // "export" dapat melakukan banyak export
        // "export" di tangkap (import) menggunakan kurung kurawal
        // "export default" cuma bisa 1 aja yg di export
        // "export default" ditangkap tanpa kurung kurawal
        export { motor, smartPhone as smartPhoneJepang}
        export default entertainment
        ```
    - script `indonesia.js`
        ```javascript
        // import dari file jepang dan amerika
        import Entertainment, { motor as motorJepang, smartPhoneJepang, sayHello } from "./jepang.js"
        import {apple} from './amerika.js';

        sayHello()

        console.log(Entertainment);
        console.log(smartPhoneJepang);

        console.log(motorJepang);

        motorJepang.splice(1, 1)

        console.log(motorJepang)
        console.log(apple);
        ```
        <br>

## **JavaScript Asynchronous**<hr>

- ### **Deskripsi**
  <div align="justify">
  Javascript adalah bahasa pemrograman single-thread yang artinya hanya dapat mengeksekusi satu task pada satu waktu atau biasa disebut synchronous. Pada konsep pemrograman (web development pada case kita) dikenal istilah Asynchronous. Asynchronous mengizinkan komputer memproses task yang lain sambil menunggu proses yang masih berlangsung.

- ### **Membuat Asynchronous**
  <div align="justify">
  Kita bisa membuat asynchronous secara simulasi artinya tidak murni asynchronous dengan beberapa cara:

    - Callback
    - Promises
    - Async/Await

- ### **Callback**
  <div align="justify">
  Callback function adalah function yang kita letakan di dalam argumen/parameter pada function, dan function tersebut akan dieksekusi setelah function pertama menyelesaikan tugasnya.

    ```javascript
    const mainFunc = (number1, number2, callBack) => {
        console.log(number1 + number2)
        callBack()
    }

    const myCallback = () => {
        console.log('Done !')
    }
    main(1,2,myCallback) // Output : 3 Done !
    ```
- ### **Promises**
  <div align="justify"> 
  Promise adalah salah satu fitur baru di ES6, biasa digunakan untuk melakukan http request/fetch data dari API.<br>

  Dalam pengambilan data, promise memiliki 3 kemungkinan state.
    - Pending(sedang dalam proses)
    - Fulfilled (berhasil)
    - Rejected (gagal)

    ```javascript
    console.log("PROMISES")
    // pembuatan promise.............
    let nontonPromise = new Promise((resolve, reject) => {
    if (true) {
        resolve("nonton terpenuhi") // berhasil
    } 

    reject("gagal"); // gagal
    });

    // eksekusi proses..............
    console.log("A");

    nontonPromise
    .then((result) => {
        console.log(result);
        return `${result} bareng doi`
    })
    .then((result) => {
        console.log(result)
    })
    .catch((err) => {
        console.log(err);
    });

    console.log("C");
    ```

- ### **Async-Await**
  <div align="justify"> 
  Async - await adalah salah satu fitur baru dari javascript yang digunakan untuk menangani hasil dari sebuah Promise. Sedangkan await berfungsi untuk menunda sebuah kode dijalankan sampai proses asynchronous berhasil.<br>
  
  Cara penulisan Async/await menggunakan es6 dan tidak menggunakan es6.
    ```javascript
    async function hello(){
        let result = await 'Hello'
        return result
    }
    // es 6
    const hello1 = async () => {
        let result = await 'hello'
        return result
    }
    ```

## **JavaScript Web Storage**<hr>

- ### **Deskripsi**
  Ada beberapa cara untuk menyimpan data pengguna seperti pencarian, artikel berita, dan lain-lain ke lokal (browser) menggunakan web storage seperti cookies, local storage, dan session storage. 

- ### **Cookies**
  <div align="justify">
  Cookies adalah data kecil yang dikirim dari situs web dan disimpan di komputer kita oleh web browser saat kita menjelajah. Disebut data kecil karena maksimum data yang dapat disimpan dalam cookies adalah 4096 bytes (4 KB). Biasanya data yang disimpan di cookies adalah access token pengguna saat login atau data pencarian saat melakukan pencarian pada situs web tertentu.

- ### **Local Storage**
  <div align="justify">
  Dengan memanfaatkan local storage dan session storage, kita dapat menyimpan data lebih besar yaitu 5MB per page tanpa mempengaruhi kinerja situs web.

   - Local storage memiliki karakteristik sebagai berikut:
     - Menyimpan data tanpa tanggal kadaluarsa.
     - Data tidak akan dihapus ketika web browser ditutup dan akan tersedia seterusnya selama kita tidak menghapus data local storage pada web browser.
     - Dapat menyimpan data hingga 5MB.
     - Hanya dapat menyimpan data string.

  - **Menyimpan data pada local storage**
    <div align="justify">
    kita menggunakan method setItem() yang membutuhkan 2 parameter. Parameter pertama adalah key yang ingin kita simpan dan parameter kedua adalah data (value) dari key yang akan disimpan.

    ```javascript
    localStorage.setItem('key', value);
    ```
  - **Mengambil data pada local storage**
    <div align="justify">
    kita dapat menggunakan method getItem() yang membutuhkan 1 parameter. Parameter tersebut adalah key dari data yang kita inginkan.

    ```javascript
    localStorage.getItem('key');
    ```

   - **Menghapus data pada local storage**
     <div align="justify">
     kita dapat menggunakan method removeItem() yang membutuhkan 1 parameter. Parameter tersebut adalah key dari data yang ingin kita hapus.

     ```javascript
     // menghapus key tertentu
     localStorage.removeItem("key");

     // menghapus semua key
     localStorage.clear();
     ```
- ### **Session Storage**
  <div align="justify">
  Berbeda dengan local storage, walaupun masuk ke dalam web storage, data yang tersimpan pada session storage akan hilang ketika session dari sebuah laman berakhir.

  - Session storage mempunyai beberapa karakteristik, yaitu:
    - Data yang disimpan pada session storage akan terus tersimpan selama browser terbuka dan tidak hilang jika laman di-reload.
    - Membuka banyak tab/window dengan URL yang sama, akan menciptakan session storage yang berbeda di masing-masing tab/window.
    - Menutup tab/window akan mengakhiri session dan menghapus data yang tersimpan di session storage pada tab/window tersebut.
    - Data yang tersimpan dalam session storage harus berbentuk string.
    - Hanya dapat menyimpan data sebanyak 5MB.

  - Sintaks untuk menyimpan data pada session storage adalah sebagai berikut:
    ```javascript
    // menambah session storage
    sessionStorage.setItem('key', value);
    ```
  - cara mendapatkan data dari session storage juga menggunakan getItem(), seperti berikut ini:
    ```javascript
    // mendapatkan session storage
    sessionStorage.getItem('key');
    ```
  - Syntax untuk menghapus data dari session storage ada 2, yaitu:
    ```javascript
    // menghapus session storage satu persatu berdasarkan key
    sessionStorage.removeItem('key');

    // menghapus seluruh session storage sekaligus
    sessionStorage.clear();
    ```

  
    


  