# Phase-0-Week-3

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

### Akses Elemen dalam Array
```javascript
let colors = ["Red", "Green", "Blue"];
console.log(colors[0]); // Output: Red
console.log(colors[1]); // Output: Green
console.log(colors[2]); // Output: Blue
```

### Menambahkan dan Menghapus Elemen
- **`push()`**: Menambahkan elemen ke akhir array
- **`pop()`**: Menghapus elemen terakhir
- **`unshift()`**: Menambahkan elemen ke awal array
- **`shift()`**: Menghapus elemen pertama

```javascript
let numbers = [1, 2, 3];
numbers.push(4);  // [1, 2, 3, 4]
numbers.pop();    // [1, 2, 3]
numbers.unshift(0); // [0, 1, 2, 3]
numbers.shift();  // [1, 2, 3]
```

### Looping dalam Array
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

### Metode Lainnya
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

### Tugas 2: Pengolahan Data dengan `map()` dan `filter()`
Buatlah array angka `[10, 15, 20, 25, 30]`, lalu:
1. Buat array baru yang berisi angka dikalikan 2 menggunakan `map()`.
2. Buat array baru yang hanya berisi angka lebih dari 20 menggunakan `filter()`.

```javascript
let numbers = [10, 15, 20, 25, 30];
// Gunakan map() dan filter()
```

Selamat belajar dan selesaikan tugas dengan baik! 🚀

