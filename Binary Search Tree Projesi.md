# **Proje 3**
`[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]` dizisinin Binary-Search-Tree aşamalarını yazınız.

## **Cevap**

Verilen dizide root olarak `7` seçilsin.

Sayıları root'un sağına ve soluna gelecek şekilde yerleştiririz. Root'un sağında rootdan daha büyük olan sayı, solundan ise küçük olan sayı bulunur.

```
            7 
             \       Root(7)'un sağında 8 vardır.
              8

```
```
            8 
             \       8'in sağında 9
              \
               9

```

```
            7 
           /         Root(7)'un solunda 5 vardır.
          5

```
```
            5 
           / \
          /   \      5'in solunda 1, sağında 6 vardır.
         1     6

```
```
            1 
           / \
          /   \      1'in solunda 1, sağında 3 vardır.
         /     \
        0       3

```
```
            3 
           / \
          /   \      3'ün solunda 2, sağında 4 vardır.
         /     \
        2       4
```

Yani en son gösterim olarak ;

```

           7          
          / \
         5   8
        / \    \            Şeklinde olacaktır. 
       1   6     9
      / \
     0   3
        /  \
       2    4
```