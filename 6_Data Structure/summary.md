# Resume Time Complexity & Space Complexity

1. Array adalah salah satu struktur data yang memiliki kelompok dari sebuah element, bisa terdapat tipe variabel dengan ukuran yang tetap. Tipe data yang berbeda dapat diatasi oleh banyak element di dalam array seperti Numeric, String, dan Boolean. Berikut contoh deklarasi sebuah array <br>
`var countries [2]string = [2]string["Jakarta", "Bandung]`<br>
`countries := [2]string["Jakarta", "Bandung]`<br>
Selain itu ada struktur data yang mirip sekali dengan array yaitu slice. Slice merupakah salah satu struktur data lainya yang dapat berisi banyak element, dapat berisi satu tipe data (seperti array) tetapi memiliki ukuran alokasi yang dinamis (tidak tetap). Berikut contoh deklarasi sebuah slice/<br>
`var primes []int = []int{2, 3, 5, 7}`<br>
`var primes []int = make([]int, 5)`<br>

3. Map merupakah struktur data yang berbentuk key dan value dimana setiap key harus unik. Berikut contoh deklarasi sebuah map.<br>
`var salary = map[string]int{"andi":20000, "umar":40000}`<br>
`salary := make(map[string]int, 5)`

4. Function adalah sepotong kode yang dapat digunakan ketika kita memanggil namanya. dengan function kita dapat dengan mudah membagi kode kedalam blok blok kecil. Hal tersebut dapat memungkinkan kita menuliskan kode dengan rapih.
Contoh function <br>
`string hello() {
    fmt.Println("Hello, My name is Restu")
}`<br>

# Task
## Problem 1 - Bilangan Prima
Dalam matematika, bilangan prima adalah bilangan asli yang lebih besar dari angka 1, yang faktor pembaginya adalah 1 dan bilangan itu sendiri. 2 dan 3 adalah bilangan prima. 4 bukan bilangan prima karena 4 bisa dibagi 2. Kamu diminta untuk membuat fungsi untuk menentukan bahwa sebuah bilangan termasuk bilangan prima atau tidak.

Buatlah solusi yang lebih optimal, dengan kompleksitas lebih cepat dari O(n) / O(n/2).
<pre>
Sample Test Cases
Input: 1000000007
Output: Bilangan Prima

Input: 1500450271
Output: Bilangan Prima
</pre>
Berikut solusi yang telah saya kerjakan 

[1.bilangan_prima.go](./praktikum/1.bilangan_prima.go)

Output :
![problem1](./screenshots/problem1.png)

## Problem 2 - Fast Exponentiation
Given two integers x and n, write a function to compute x^n. We may assume that x and n are small and overflow doesn’t happen.

Create optimal solution with time complexity more fast that O(n). -> logarithmic
<pre>
Sample Test Cases
Input : x = 2, n = 3
Output : 8

Input : x = 7, n = 2
Output : 49
</pre>
Berikut solusi yang telah saya buat 

[2.fast_exponentiation.go](./praktikum/2.fast_exponentiation.go)

Output :
![problem2](./screenshots/problem2.png)

## Problem 3 - Array Merge
Problem 3 - Array Merge
Buatlah sebuah program menggabungkan 2 array yang diberikan, dan jangan sampai terdapat nama yang sama di data yang sudah tergabung tadi. (Structure Data , No BruteForce)
<pre>
Sample Test Cases
Input: ['kazuya', 'jin', 'lee'], ['kazuya', 'feng']
Output: ['kazuya', 'jin', 'lee', 'feng']

Input: ['lee', 'jin'], ['kazuya', 'panda']
Output: ['lee', 'jin', 'kazuya', 'panda']
</pre>

Berikut solusi yang telah saya buat 

[3.array_merge.go](./praktikum/3.array_merge.go)

Output: 
![problem3](./screenshots/problem3.png)

## Problem 4 - Angka Muncul Sekali

Buat program sesuai dengan deskripsi di bawah. Input merupakan variable string berisi kumpulan angka. Output merupakan list / array berisi angka yang hanya muncul 1 kali pada input.
<pre>
Sample Test Case

Input: “76523752”
Output: [6, 3]

Input: “1122”
Output: []
</pre>

Berikut solusi yang telah saya buat

[4.angka_muncul_sekali.go](./praktikum/4.angka_muncul_sekali.go)

Output:
![problem4.go](./screenshots/problem4.png)

## Problem 5 - Pair With Target Sum
Given an array of sorted numbers and a target sum, find a pair in the array whose sum is equal to the given target.

Write a function to return the indices of the two numbers (i.e. the pair) such that they add up to the given target.

Challenges:
Solve with linear complexity O(n), not O(n^2) if you can!
<pre>
Sample Test Cases
Input: [1, 2, 3, 4, 6], target=6
Output: [1, 3]
Explanation: The numbers at index 1 and 3 add up to 6: 2+4=6

Input: [2, 5, 9, 11], target=11
Output: [0, 2]
Explanation: The numbers at index 0 and 2 add up to 11: 2+9=11
</pre>

Berikut solusi yang telah saya buat 

[5.pair_with_target_sum.go](./praktikum/5.pair_with_target_sum.go)

Output:
![problem5](./screenshots/problem5.png)