# Data-Structures-Algorithms
Data Structures and Algorithms

1. [22,27,16,2,18,6] (Başlangıç)
2. [22,27,16,2,18,6] (22<27 doğru sırada)
3. [22,16,27,2,18,6] -> [16,22,27,2,18,6]
4. [16,22,2,27,18,6] -> [16,2,22,27,18,6] -> [2,16,22,27,18,6]
5. [2,16,22,18,27,6] -> [2,16,18,22,27,6]
6. [2,16,18,22,6,27] -> [2,16,18,6,22,27] -> [2,16,6,18,22,27] -> [2,6,16,18,22,27]
Big-O Gösterimi: O(n²)
Time Complexity:
18 sayısı dizinin ortalarında bulunduğu için Average Case kapsamına girer.
[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımı:
1. [2,3,5,8,7,9,4,15,6] (En küçük sayı 2 bulunur ve başa getirilir)
2. [2,3,5,8,7,9,4,15,6] (3 zaten doğru konumda)
3. [2,3,4,8,7,9,5,15,6] (4 bulunur ve 3. sıraya getirilir)
4. [2,3,4,5,7,9,8,15,6] (5 bulunur ve 4. sıraya getirilir)
   
Bölme Aşamaları:
                   [16,21,11,8,12,22]
                /                \
        [16,21,11]            [8,12,22]
        /         \           /        \
    [16]    [21,11]       [8]     [12,22]
     |      /     \        |      /      \
    [16]  [21]   [11]    [8]   [12]    [22]

Birleştirme Aşamaları:
      [16]  [11,21]    [8]   [12,22]
     |      |         |       |
    [11,16,21]      [8,12,22]
           \         /
      [8,11,12,16,21,22]

Detaylı birleştirme adımları:
[21] ve [11] -> [11,21]
[16] ve [11,21] -> [11,16,21]
[12] ve [22] -> [12,22]
[8] ve [12,22] -> [8,12,22]
[11,16,21] ve [8,12,22] -> [8,11,12,16,21,22]

Big-O Gösterimi: O(nlog n)

[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary Search Tree aşamaları:


1. Root 7'dir.
2. Her düğümde, sol taraf kendinden küçük, sağ taraf kendinden büyük değerleri içerir.                7
               / \
              5   8
             / \   \
            1   6   9
           / \
          0   3
             / \
            2   4

Özellikler:
Her düğümün solundaki tüm değerler kendinden küçük
Her düğümün sağındaki tüm değerler kendinden büyük
Her düğümün en fazla 2 çocuğu olabilir
Aynı değer ağaçta tekrar bulunamaz
