# iteration(loop)

Repository ini berisi pembelajaran dasar tentang **Iteration (Loop)** dalam pemrograman menggunakan Python.

Loop digunakan untuk menjalankan perintah secara berulang tanpa harus menulis kode yang sama berkali-kali.

---

# Pengertian Iteration (Loop)

Iteration atau loop adalah proses pengulangan suatu instruksi sampai kondisi tertentu terpenuhi.

Dalam pemrograman, loop sangat penting karena:
- Menghemat penulisan kode
- Membuat program lebih efisien
- Mempermudah pengolahan data
- Mengurangi pengulangan manual

---

# Kenapa Harus Menggunakan Loop?

Bayangkan ingin menampilkan angka 1 sampai 100.

Tanpa loop:
```python
print(1)
print(2)
print(3)
...
print(100)
```

Sangat panjang dan tidak efisien.

Dengan loop:
```python
for i in range(1, 101):
    print(i)
```

Lebih singkat, rapi, dan mudah dipahami.

---

# Jenis-Jenis Loop di Python

## 1. For Loop

`for` digunakan untuk mengulang berdasarkan jumlah data atau range tertentu.

### Struktur Dasar
```python
for variabel in range():
    perintah
```

---

## Contoh For Loop

### Menampilkan angka 1 sampai 5
```python
for i in range(1, 6):
    print(i)
```

### Output
```python
1
2
3
4
5
```

---

## Penjelasan

- `i` → variabel perulangan
- `range(1, 6)` → dimulai dari 1 sampai sebelum 6
- `print(i)` → menampilkan nilai i

---

# Fungsi range()

`range()` digunakan untuk menentukan jumlah perulangan.

## Bentuk range()

### 1. range(stop)
```python
range(5)
```

Output:
```python
0 1 2 3 4
```

---

### 2. range(start, stop)
```python
range(1, 6)
```

Output:
```python
1 2 3 4 5
```

---

### 3. range(start, stop, step)
```python
range(2, 11, 2)
```

Output:
```python
2 4 6 8 10
```

---

# 2. While Loop

`while` digunakan untuk mengulang selama kondisi bernilai True.

---

## Struktur Dasar
```python
while kondisi:
    perintah
```

---

## Contoh While Loop

```python
angka = 1

while angka <= 5:
    print(angka)
    angka += 1
```

### Output
```python
1
2
3
4
5
```

---

## Penjelasan

- `angka = 1` → nilai awal
- `while angka <= 5` → perulangan berjalan selama kondisi benar
- `angka += 1` → menambah nilai angka setiap loop

Jika tidak ada penambahan nilai, loop bisa berjalan terus menerus (infinite loop).

---

# Infinite Loop

Infinite loop adalah loop yang tidak berhenti karena kondisi selalu True.

## Contoh
```python
while True:
    print("Hello")
```

Loop di atas akan terus berjalan sampai program dihentikan manual.

---

# Break

`break` digunakan untuk menghentikan loop.

## Contoh
```python
for i in range(1, 11):
    if i == 5:
        break

    print(i)
```

### Output
```python
1
2
3
4
```

---

# Continue

`continue` digunakan untuk melewati satu perulangan.

## Contoh
```python
for i in range(1, 6):
    if i == 3:
        continue

    print(i)
```

### Output
```python
1
2
4
5
```

---

# Nested Loop

Nested loop adalah loop di dalam loop.

## Contoh
```python
for i in range(3):
    for j in range(3):
        print(i, j)
```

### Output
```python
0 0
0 1
0 2
1 0
1 1
1 2
2 0
2 1
2 2
```

---

# Contoh Kehidupan Sehari-hari

## Menghitung Mundur

```python
for i in range(5, 0, -1):
    print(i)
```

### Output
```python
5
4
3
2
1
```

---

## Menampilkan Nama Berulang

```python
for i in range(3):
    print("Python")
```

### Output
```python
Python
Python
Python
```

---

# Kelebihan Loop

- Mempercepat penulisan program
- Mengurangi duplikasi kode
- Membuat program lebih fleksibel
- Mempermudah pengolahan data dalam jumlah banyak

---

# Kesalahan Umum Saat Menggunakan Loop

## 1. Infinite Loop
Loop tidak berhenti karena kondisi selalu benar.

## 2. Salah Indentasi
Python menggunakan indentasi untuk menentukan blok kode.

Contoh salah:
```python
for i in range(5):
print(i)
```

Contoh benar:
```python
for i in range(5):
    print(i)
```

---

# Kesimpulan

Iteration (Loop) adalah konsep penting dalam pemrograman untuk melakukan pengulangan secara otomatis.

Jenis loop utama di Python:
- `for`
- `while`

Loop membantu membuat kode:
- Lebih singkat
- Lebih rapi
- Lebih efisien

---

# Referensi

- https://docs.python.org
- https://www.w3schools.com/python/
- https://www.geeksforgeeks.org/python-loops/

---

# Author

Belajar pemrograman dari nol 🚀
