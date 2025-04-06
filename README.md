}

# JavaScript Week 3: Arrays

## 1. Array dalam JavaScript

### Penjelasan
Array adalah struktur data yang digunakan untuk menyimpan kumpulan nilai dalam satu variabel. Setiap nilai dalam array memiliki indeks yang dimulai dari 0.

Array dapat menyimpan berbagai tipe data seperti string, number, boolean, bahkan array atau objek lainnya.

### Cara Membuat Array
1. **Menggunakan Bracket (`[]`)**
   ```javascript
   let fruits = ["Apple", "Banana", "Cherry"];
   ```
2. **Menggunakan `new Array()`**
   ```javascript
   let numbers = new Array(1, 2, 3, 4, 5);
   ```

---

## 2. Contoh Penggunaan

### Properti Panjang Array
`.length`

Membaca jumlah elemen yang ada dalam suatu array:

```javascript
let arr = [10, 20, 30];
console.log(arr.length); // 3
```

### Akses Elemen dalam Array
```javascript
let colors = ["Red", "Green", "Blue"];
console.log(colors[0]); // Output: Red
console.log(colors[1]); // Output: Green
console.log(colors[2]); // Output: Blue
```

### Menambahkan dan Menghapus Elemen
- **`push()`**: Menambahkan elemen ke akhir array
- **`pop()`**: Mengambil elemen terakhir
- **`unshift()`**: Menambahkan elemen ke awal array
- **`shift()`**: Mengambil elemen pertama

```javascript
let numbers = [1, 2, 3];
numbers.push(4);  // [1, 2, 3, 4]
numbers.pop();    // [1, 2, 3]
numbers.unshift(0); // [0, 1, 2, 3]
numbers.shift();  // [1, 2, 3]
```

### Looping dalam Array
Menggunakan **for**:
```javascript
let animals = ["Cat", "Dog", "Elephant"];
for (let i = 0; i < animals.length; i++) {
  console.log(animals[i]);
}
```

Menggunakan **forEach()**:
```javascript
let animals = ["Cat", "Dog", "Elephant"];
animals.forEach((animal) => {
    console.log(animal);
});
```

Menggunakan **for-of**:
```javascript
for (let animal of animals) {
    console.log(animal);
}
```

### Fungsi Pencarian Indeks dan Elemen
- **`indexOf()`** – Mengetahui indeks keberapa dari suatu elemen
- **`includes()`** – Memastikan keberadaan suatu elemen
```javascript
let items = ["pen", "book", "notebook"];

console.log(items.indexOf("book")); // 1
console.log(items.includes("pen")); // true
```

### Fungsi Menyisip dan Mengiris
- **`splice()`** – Menghapus dan menyisipkan elemen-elemen pada suatu indeks
- **`slice()`** – Menyalin sebagian elemen-elemen dari suatu array
```javascript
let arr = ["a", "b", "c", "d"];

// splice(start, deleteCount, item1, item2, ...)
arr.splice(1, 2, "x", "y"); // ["a", "x", "y", "d"]

// slice(start, end)
let newArr = arr.slice(1, 3); // ["x", "y"]

```

### Fungsi Lainnya
- **`map()`** – Membuat array baru dengan hasil operasi pada setiap elemen
- **`filter()`** – Menyaring elemen berdasarkan kondisi tertentu
- **`reduce()`** – Mengakumulasikan nilai array menjadi satu nilai

```javascript
let numbers = [1, 2, 3, 4, 5];
let squared = numbers.map(num => num * num); // [1, 4, 9, 16, 25]

let evenNumbers = numbers.filter(num => num % 2 === 0); // [2, 4]

let sum = numbers.reduce((total, num) => total + num, 0); // 15
```

---

## 3. Assignment

### Tugas 1: Manipulasi Array
Buatlah array bernama `students` yang berisi daftar nama siswa. Tambahkan satu nama baru, hapus nama pertama, lalu cetak hasil akhirnya.

```javascript
let students = ["Alice", "Bob", "Charlie"];
// Lakukan manipulasi array di sini
```

### Tugas 2: Mencari Bilangan Terbesar
Buatlah fungsi yang dapat mencari bilangan terbesar dari suatu array:
```javascript
function getMax(arr) {
  return Math.max(...arr);
}

console.log(getMax([4, 10, 2, 99])); // 99
```

### Tugas 3: Pengolahan Data dengan `map()` dan `filter()`
Buatlah array angka `[10, 15, 20, 25, 30]`, lalu:
1. Buat array baru yang berisi angka dikalikan 2 menggunakan `map()`.
2. Buat array baru yang hanya berisi angka lebih dari 20 menggunakan `filter()`.

```javascript
let numbers = [10, 15, 20, 25, 30];
// Gunakan map() dan filter()
```

Selamat belajar dan selesaikan tugas dengan baik! 🚀

