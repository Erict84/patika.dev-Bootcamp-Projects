## Proje 1

> **[22,27,16,2,18,6]** → Insertion Sort
> Yukarida verilen dizinin sort turune gore asamalarini yaziniz. 
> Big-O gosterimini yaziniz. 
> Time Complexity: Diz siralandiktan sonra 18 sayisi asagidaki case’lerden hangisinin kapsamina girer? Yaziniz. 
> 1. Average case: Aradigimiz sayinin ortada olmasi
> 2. Worst case: Aradigimiz sayinin sonda olmasi
> 3. Best case: Aradigimiz sayinin dizinin en basinda olmasi
>
> **[7,3,5,8,2,9,4,15,6]** dizisinin Selection Sort’a gore ilk 4 adimini yaziniz.
> 

### Dizinin sorting asamalari:

**Step-1** : [ **22** , 27 , 16 , **2** , 18 , 6 ] → [ **2** , 27 , 16 , **22** , 18 , 6 ] Yapilan islem sayisi: (**n** = 6)

**Step-2** : [ 2 , **27** , 16 , 22 , 18 , **6** ] → [ 2 , 6 , 16 , 22 , 18 , 27 ] Yapilan islem sayisi: (**n-1** = 5)

**Step-3** : [ 2 , 6 , **16** , 22 , 18 , 27 ] → [ 2 , 6 , 16 , 22 , 18 , 27 ] Yapilan islem sayisi: (**n-2** = 4)

**Step-4** : [ 2 , 6 , 16 , **22** , **18** , 27 ] → [ 2 , 6 , 16 , 18 , 22 , 27 ] Yapilan islem sayisi: (**n-3** = 3)

**Step-5** : [ 2 , 6 , 16 , 18 , **22** , 27 ] → [ 2 , 6 , 16 , 18 , 22 , 27 ] Yapilan islem sayisi: (**n-4** = 2)

**Step-6** : [ 2 , 6 , 16 , 18 , 22 , **27** ] → [ 2 , 6 , 16 , 18 , 22 , 27 ] Yapilan islem sayisi: (**n-5** = 1)

### Sorting Big-O Gosterimi:

**Yapilan islem sayisi**: $(n + (n-1) + (n-2) + ... ) = ( n * (n + 1) / 2) = ( (n^2 + n ) /2)$  

$$
Big-O(n^2)
$$

### Time Complexity:

Dizi siralandiktan sonra: [ 2 , 6 , 16 , 18 , 22 , 27 ] 18 sayisi dizinin ortasinda yer aldigi icin 

<aside>
🔥 18 → Average Case

</aside>

### **[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort’a gore ilk 4 adimi:**

**Step-1 :** [ **7** , 3 , 5 , 8 , **2** , 9 , 4 , 15 , 6 ] → [ **2** , 3 , 5 , 8 , **7** , 9 , 4 , 15 , 6 ] 

**Step-2** : [ **2** , **3** , 5 , 8 , 7 , 9 , 4 , 15 , 6 ] → [ **2** , **3** , 5 , 8 , 7 , 9 , 4 , 15 , 6 ]

**Step-3 :** [ **2** , **3** , **5** , 8 , 7 , 9 , **4** , 15 , 6 ] → [ **2** , **3** , **4** , 8 , 7 , 9 , **5** , 15 , 6 ]

**Step-4 :** [ **2** , **3** , **4** , **8** , 7 , 9 , **5** , 15 , 6 ] → [ **2** , **3** , **4** , **5** , 7 , 9 , **8** , 15 , 6 ]

Dizideki en kucuk eleman bulunarak en bastaki elemanla yer degistirilir, ve yerlestirilen eleman sabitlenir. Kirmizi ile isaretlenenler sabitlenen elemanlardir. Ayni islemi kalan elemanlar tamamen sabitlenene kadar tekrarlariz.
