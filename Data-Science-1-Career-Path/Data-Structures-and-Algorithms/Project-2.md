> **[16,21,11,8,12,22]** -> Merge Sort
>
> * Yukarıdaki dizinin sort türüne göre aşamalarını yazınız. 
> * Big-O gösterimini yazınız.
> 

### Merge Sort Aşamaları

**Step-1 :** [ 16 , 21 , 11 ]                  [ 8 , 12 , 22 ]

**Step-2 :** [ 16 ] [ 21 , 11 ]               [ 8 ] [ 12 , 22 ]

**Step-3 :** [ 16 ] [ 21 ] [ 11 ]            [ 8 ] [ 12 ] [ 22 ]

**Step-4 :** [ 16 ] [ 11 , 21 ].              [ 8 ] [ 12 , 22 ]

**Step-5 :** [ 11 , 16 , 21 ]                  [ 8 , 12 , 22 ]

**Step-6 :** [ 8 , 11 , 12 , 16 , 21 , 22 ]

Totalde yapacagimiz islem sayisi $2^x = n => x = log(n)$ dir. Bu nedenle: 

$Big-O(log(n))$ 

olarak gosterilir.
