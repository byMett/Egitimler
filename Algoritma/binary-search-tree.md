
### [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.
##### Binary Search Tree, node’lardan oluşan ve her bir node’un en fazla 2 child node’a sahip olduğu veri yapılarından bir tanesidir.

|     Açıklama    |  |  |  |
|--               |- |- |- |
|**root=7**       |  | 7|  |



** "5" rakamı "7" rakamından küçük olduğundan 7'nin soluna ekledik**
|   Açıklama  |     |  |  |
|--           |-    |- |- |
|             |     |  | 7|  
|             |     | /|  | 
|**5 ekledik**|**5**|  |  | 


**"1" rakamı "5" rakamından ve 7'den küçük olduğundan 7 ve 5'in soluna ekledik** 
|     Açıklama  |     |  |  |  |  |
|             --|--   |--|- |- |- |
|               |     |  |  |  | 7|  
|               |     |  |  | /|  | 
|               |     |  | 5|  |  |  
|               |     | /|  |  |  | 
|**1 ekledik**  |**1**|  |  |  |  |

**"8" rakamı "7" rakamından büyük olduğundan 7'nin sağına ekledik** 
| Açıklama      |  |  |  |  |  |  |     |
|--             |--|--|- |- |- |- |-    |
|               |  |  |  |  | 7|  |     |  
|               |  |  |  | /|  |\ |     | 
|**8 ekledik**  |  |  | 5|  |  |  |**8**| 
|               |  | /|  |  |  |  |     | 
|               | 1|  |  |  |  |  |     |

**"3" rakamı  "7" ve "5" rakamından küçük  olduğundan 5'in soluna, 1'den büyük olduğundan 1'in sağına ekledik**  
|  Açıklama     |  |  |     |  |  |  |  |
|--             |--|--|-    |- |- |- |- |
|               |  |  |     |  | 7|  |  |  
|               |  |  |     | /|  |\ |  | 
|               |  |  | 5   |  |  |  |8 | 
|               |  | /|     |  |  |  |  | 
|               | 1|  |     |  |  |  |  |
|               |  |\ |     |  |  |  |  |
|**3 ekledik**  |  |  |**3**|  |  |  |  |

**"6" rakamı "7" rakamından küçük  olduğundan 7'nin soluna, "5" rakamından büyük olduğundan 5'in sağına ekledik**  
| Açıklama      |  |  |  |  |     |  |  |
|--             |--|--|- |- |-    |- |- |
|               |  |  |  |  | 7   |  |  |  
|               |  |  |  | /|     |\ |  | 
|               |  |  | 5|  |     |  |8 | 
|               |  | /|  |\ |     |  |  | 
| **6 ekledik** | 1|  |  |  |**6**|  |  |
|               |  |\ |  |  |     |  |  |
|               |  |  | 3|  |     |  |  |

**"0" "7" rakamından, "5" ve "1" rakamından küçük  olduğundan 1'in soluna ekledik**  
| Açıklama       |     |  |  |  |  |  |  |  |  |
|--              |--   |--|- |- |- |- |- |- |- |
|                |     |  |  |  |  |  | 7|  |  |  
|                |     |  |  |  |  | /|  |\ |  | 
|                |     |  |  |  | 5|  |  |  |8 | 
|                |     |  |  | /|  |\ |  |  |  |
|                |     |  | 1|  |  |  |6 |  |  |
|                |     | /|  |\ |  |  |  |  |  |
| **0 ekledik**  |**0**|  |  |  | 3|  |  |  |  |

**"9" rakamı  "7" ve "8" rakamından büyük olduğundan  8'in sağına ekledik**  
| Açıklama     |  |  |  |  |  |  |  |  |  |  |     |
|--            |--|--|- |- |- |- |- |- |- |- |-    |
|              |  |  |  |  |  |  | 7|  |  |  |     |  
|              |  |  |  |  |  | /|  |\ |  |  |     | 
|              |  |  |  |  | 5|  |  |  |8 |  |     | 
|              |  |  |  | /|  |\ |  |  |  |\ |     | 
| **9 ekledik**|  |  | 1|  |  |  |6 |  |  |  |**9**|
|              |  | /|  |\ |  |  |  |  |  |  |     |
|              | 0|  |  |  | 3|  |  |  |  |  |     |


**"4" rakamı  "7" ve "5" rakamından küçük olduğundan 5'in soluna, "1" ve "3" rakamından büyük olduğundan 3'ün sağına ekledik** 
| Açıklama    |  |  |  |  |  |  |     |  |  |  |  |
|--           |--|--|- |- |- |- |-    |- |- |- |- |
|             |  |  |  |  |  |  | 7   |  |  |  |  |  
|             |  |  |  |  |  | /|     |\ |  |  |  | 
|             |  |  |  |  | 5|  |     |  |8 |  |  | 
|             |  |  |  | /|  |\ |     |  |  |\ |  |
|             |  |  | 1|  |  |  |6    |  |  |  | 9|
|             |  | /|  |\ |  |  |     |  |  |  |  |
|             | 0|  |  |  | 3|  |     |  |  |  |  |
|             |  |  |  |  |  |\ |     |  |  |  |  |
|**4 ekledik**|  |  |  |  |  |  |**4**|  |  |  |  |

**"2" rakamı "7" ve "5" rakamından küçük olduğundan 5'in soluna, "1" rakamından büyük olduğundan 1'in sağına ve 3'ten küçük olduğunda 3'ün soluna ekledik** 
| Açıklama    |  |  |     |  |  |  |  |  |  |  |  |
|--           |--|--|-    |- |- |- |- |- |- |- |- |
|             |  |  |     |  |  |  | 7|  |  |  |  |  
|             |  |  |     |  |  | /|  |\ |  |  |  | 
|             |  |  |     |  | 5|  |  |  |8 |  |  | 
|             |  |  |     | /|  |\ |  |  |  |\ |  | 
|             |  |  | 1   |  |  |  |6 |  |  |  | 9|
|             |  | /|     |\ |  |  |  |  |  |  |  |
|             | 0|  |     |  | 3|  |  |  |  |  |  |
|             |  |  |     | /|  |\ |  |  |  |  |  |
|**2 ekledik**|  |  |**2**|  |  |  |4 |  |  |  |  |