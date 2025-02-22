# mergesort
Swift eğitimimin bir parçası olan Algoritma ve Veri Yapıları merge sort konusu icin bir örnek çözüm.

### Adım Adım **Merge Sort** Aşamaları:

Verilen dizi: **[16, 21, 11, 8, 12, 22]**

1. **Diziyi ikiye bölelim:**
    - [16, 21, 11] ve [8, 12, 22]
2. **İlk yarıyı sıralayalım (Merge Sort ile):**
    - [16, 21, 11] dizisini ikiye bölelim: [16] ve [21, 11]
    - [21, 11] dizisini ikiye bölelim: [21] ve [11]
    - [21] ve [11] dizilerini karşılaştırıp birleştirelim: [11, 21]
    - Şimdi [16] ve [11, 21] dizilerini karşılaştıralım ve sıralayalım: [11, 16, 21]
3. **İkinci yarıyı sıralayalım (Merge Sort ile):**
    - [8, 12, 22] dizisini ikiye bölelim: [8] ve [12, 22]
    - [12, 22] dizisini ikiye bölelim: [12] ve [22]
    - [12] ve [22] dizilerini karşılaştırıp birleştirelim: [12, 22]
    - Şimdi [8] ve [12, 22] dizilerini karşılaştıralım ve sıralayalım: [8, 12, 22]
4. **Şimdi sıralı iki yarıyı birleştirelim:**
    - [11, 16, 21] ve [8, 12, 22] dizilerini karşılaştırıp sıralayalım: [8, 11, 12, 16, 21, 22]

Sonuç: **[8, 11, 12, 16, 21, 22]**

---

### **Big-O Gösterimi:**

- Merge Sort, her adımda diziyi ikiye böldüğü için **logaritmik** bir karmaşıklığa sahiptir.
- Her bir bölme işleminde, dizinin her elemanını karşılaştırıp birleştirmek gerekeceği için her bölme işlemi **O(n)**karmaşıklığına sahiptir.

Bu nedenle **Merge Sort**'un zaman karmaşıklığı: **O(n log n)**
