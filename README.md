# analizCprogVerilen
verilen kodda degisiklik

Kodun ne işe yaradığını ve nasıl çalıştığını açıklayın:
Bu kod, belirli işlevler gerçekleştiren bir C dilinde yazılmış programdır. Programın genel işleyişi aşağıdaki gibi özetlenebilir:

Program öncelikle, A_SIZE (20) büyüklüğünde bir tam sayı dizisi 'a' oluşturur ve bu diziyi rastgele sayılarla doldurur. Rastgele sayılar -MAX_W (-10) ile MAX_W (10) arasında olacak şekilde belirlenir.

Daha sonra bu diziyi bir sıralama işleminden geçirir (function1). Bu işlem, dizi elemanlarını küçükten büyüğe doğru sıralar. Bu, kabarcık sıralama (bubble sort) algoritması kullanılarak gerçekleştirilir.

Program, sıralanmış 'a' dizisini işleyerek bir 't' değeri hesaplar (function2). Bu işlem, dizi boyunca olumlu bir toplamı sürdürebileceği maksimum alt dizinin ortalamasını bulmayı içerir.

Program, bir graf temsili olan 'g' matrisini işler ve bu matris üzerinde Floyd-Warshall algoritması uygulanarak her düğüm arasındaki en kısa yolun uzunluğunu hesaplar (function3). Bu, 'd' adlı yeni bir matrise kaydedilir.

Son olarak, 't' değerinden küçük olan tüm 'd' matrisi değerlerini (yani, 't' değerinden daha kısa olan tüm yolları) yazdırır (print3).

Programın işlem süresini de ölçer ve bunu saniye cinsinden yazdırır.

Her bir işlem ayrı bir fonksiyon olarak tanımlanmıştır ve bu kodun genel amacı, belirli bir işlem kümesini gerçekleştirmek ve çıktıları yazdırmaktır. Ayrıca bu kod, çeşitli algoritmaların (kabarcık sıralama, maksimum alt dizi toplamı bulma, Floyd-Warshall algoritması) uygulanmasında bir örnektir.



Kodun zaman karmaşıklığını adım adım göstererek hesaplayın:
zaman karmaşıklığı:
1.	generate işlevi:
•	for döngüsü, size kez çalışır.
•	Her bir döngü adımında bir atama işlemi yapılır.
•	Bu nedenle, zaman karmaşıklığı O(size) veya daha doğru bir ifadeyle O(A_SIZE) olur.
2.	function1 işlevi:
•	İç içe iki for döngüsü kullanılır, her biri size-1 kez çalışır.
•	Karşılaştırma ve yer değiştirme işlemleri yapılır.
•	Bu nedenle, zaman karmaşıklığı O(size^2) veya daha doğru bir ifadeyle O(A_SIZE^2) olur.
3.	function2 işlevi:
•	Bir for döngüsü kullanılır, size kez çalışır.
•	İçerisindeki if-else yapısı sabit bir zaman karmaşıklığına sahiptir.
•	Bu nedenle, zaman karmaşıklığı O(size) veya daha doğru bir ifadeyle O(A_SIZE) olur.
4.	function3 işlevi:
•	İki adet for döngüsü kullanılır, her biri size kez çalışır.
•	İç içe bir for döngüsü daha bulunur, bu da size kez çalışır.
•	İçerisindeki if-else yapısı sabit bir zaman karmaşıklığına sahiptir.
•	Bu nedenle, zaman karmaşıklığı O(size^3) veya daha doğru bir ifadeyle O(G_SIZE^3) olur.
5.	print1 işlevi:
•	Bir for döngüsü kullanılır, size kez çalışır.
•	Her bir döngü adımında bir printf işlemi yapılır.
•	Bu nedenle, zaman karmaşıklığı O(size) veya daha doğru bir ifadeyle O(A_SIZE) olur.
6.	print2 işlevi:
•	İki adet for döngüsü kullanılır, her biri size kez çalışır.
•	Her bir döngü adımında bir printf işlemi yapılır.
•	Bu nedenle, zaman karmaşıklığı O(size^2) veya daha doğru bir ifadeyle O(G_SIZE^2) olur.
7.	print3 işlevi:
•	İki adet for döngüsü kullanılır, her biri size kez çalışır.
•	Her bir döngü adımında bir printf işlemi yapılır.
•	Bu nedenle, zaman karmaşıklığı O(size^2) veya daha doğru bir ifadeyle O(G_SIZE^2) olur.
