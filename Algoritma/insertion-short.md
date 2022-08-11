# Proje-1
### [22,27,16,2,18,6] -> Insertion Sort

##### 1. Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

Insertion Sort yani araya ekleme sıralama algoritması ikinci elemandan başlayarak elemanın kendinden önceki elemanlarla karşılaştırılması suretiyle büyük elemanların dizide sağa doğru kaydırılması işlemlerini tekrar eder.
   
Dizinin en solundan başlıyoruz. "22" kendi başına sıralıdır. Hiç bir işlem yapmıyoruz.
|1.Adım|22|27|16|2|18|6|     
|------|- |- |- |-|- |-|
    
"22" verisi ve "27" verisi karşılaştırma yapılır. "22", "27" sayısından küçük olduğu için ilk iki veri tamamlanır. Herhangi bir değişiklik yapmıyoruz.
|2.Adım|22|27|16|2|18|6|     
|------|- |- |- |-|- |-|  
         |  | 
         ---- 

"16" sayısı solundaki "27" sayısından daha düşük olduğu için bir yana kayar. Daha sonra oluşan yeni yapıda tekrar bakıyoruz. "16" sayısı  "22" sayısından küçük olduğu için yeni yerini alır.
|3.Adım|22|16|27|2|18|6|-->|16|22|27|2|18|6| 
|------|- |- |- |-|- |-|---|- |- |- |-|- |-|
            |  |            |   |         
            ----            -----

"2" rakamı ile başlıyoruz. Solundaki "27" rakamı ile karşılaştırıldında daha küçük olduğu için sola kayarak devam ediyor. En sonunda en küçük değer olarak en sola yerleşiyor.
|4.Adım|16|22|2|27|18|6|-->|16|2|22|27|18|6| 
|------|- |- |- |-|- |-|--|- |- |- |-|- |-|
               |  |            |   |
               ----            ----

|-->|2|16|22|27|18|6|
|-|- |- |- |-|- |-|
    |  | 
    ----

Ve İşlemler en küçüklerini sıralayarak devam etmektedir...

|5.Adım|2|16|22|18|27|6|-->|2|16|18|22|27|6|
|------|- |- |- |-|- |-|---|- |- |- |-|- |-|
   
|6.Adım|2|16|18|22|6|27|-->|2|16|18|6|22|27|
|------|- |- |- |-|- |-|-------|- |- |- |-|- |-|
    
|6.Adım|2|16|6|18|22|27|-->|2|6|16|18|22|27|
|------|- |- |- |-|- |-|-------|- |- |- |-|- |-|
     

     
##### 2. Big-O gösterimini yazınız.

   O(n^2)

##### 3. Time Complexity: 
###### - Worst Case: Aradığımız sayının sonda olması,
Tam ters verilmiş dizi, dizinin her bir elemanı bir öncekinden küçük olacaktır. Dolayısıyla birinci eleman için iç döngü "0 2" eleman için geriye doğru "1, 3" eleman için iki daha sonra "3 4 5 6… n" kadar geriye hareket yapacaktır. Yani "0+1+2+3+4…..+n-1 = [n*(n-1)]/2   :  n^2"

###### - Average Case: Aradığımız sayının ortada olması,
Worst Case ile Best Case'in ortalamasını aldığımızda "n^2" olarak buluruz.

###### - Best case: Aradığımız sayının dizinin en başında olması.
Tam sıralı dizi, n tane sayinin üzerinden birer defa geçer ve hiç birini geriye doğru ilerletme gereği olmadığı için bu tek geçişle kalır. Yani "n"

##### 4. Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.
Average Case kapsamına girer.
    
#### 2. [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.
 |1.Adım|7|3|5|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |2.Adım|3|7|5|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |3.Adım|3|5|7|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |4.Adım|3|5|7|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|