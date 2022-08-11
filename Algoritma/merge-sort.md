
### [16,21,11,8,12,22] -> Merge Sort

#### 1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
###### Merge Sort (Birleştirme Sıralaması), diziyi ardışık olarak en küçük alt dizilerine kadar yarılayan sonra da onları sıraya koyarak bireştiren özyineli bir algoritmadır. Yarılama işlemi en büyük alt dizi en çok iki öğeli olana kadar sürer. Sonra "Merge (Birleştirme)" işlemiyle altdiziler ikişer ikişer bölünüş sırasıyla sıralı olarak bir üst dizide bireşir. Süreç sonunda en üstte sıralı diziye ulaşılır.

|                                                 |

|Diziyi ikiye bölerek yeniden yazıyoruz           |  |  |  | 16 | 21 | 11 | 8 | 12 | 22 |  |  |  |
|                                                 
|Sol ve sağdaki dizileri tekrar ikiye böluyoruz.  |  |  | 16 | 21 | 11 |  |  | 8 | 12 | 22 |  |  |

|Tek eleman kalana kadar bir kez daha bölüyoruz.  |  | 16 | 21 |  | 11 |  |  | 8 |  | 12 | 22 |  |

|                                                 | 16 |  | 21 |  | 11 |  |  | 8 |  | 12 |  | 22 |


######  Bölme işlemi bitikten sonra, tek elemanlı dizilerimizi ikili ikili birleştiriyoruz. Sıralı dizi elde edinceye kadar bu işleme devam ediyoruz.


|                                                | 16 |  | 21 |  | 11 |  |  | 8 |  | 12 |  | 22 |

|ikili ikili ikili sıralayarak birleştiriyoruz.  |  | 16 | 21 |  | 11 |  |  | 8 |  | 12 | 22 |  |

|Tekrar ikili ikili sıralayarak birleştiriyoruz. |  |  | 11 | 16 | 21 |  |  | 8 | 12 | 22 |  |  |

|Son birleştirmede dizimizi elde ediyoruz.       |  |  |  | 8 | 11 | 12 | 16 | 21 | 22 |  |  |  |
    

#### 2. Big-O gösterimini yazınız.
Her bölünmüş dizinin Merge işlemi için de dizinin uzunluğu olan n işlem yapıldığından O(n*(logn)) --> O(6*(log6)) olacaktır.