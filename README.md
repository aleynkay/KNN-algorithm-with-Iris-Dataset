# KNN (K-Nearest Neighbors) algoritması

Temel Prensipler
KNN algoritması, yeni bir veri noktasının sınıfını veya değerini tahmin etmek için eğitim veri kümesindeki en yakın 
𝐾
K komşusunu kullanır. Bu komşuların sınıflarına veya değerlerine bakarak tahmin yapılır. Algoritmanın temel adımları şu şekildedir:

Mesafe Ölçümü: Yeni bir veri noktasının eğitim verisindeki diğer veri noktalarına olan mesafesi hesaplanır. En yaygın kullanılan mesafe ölçümü Öklidyen mesafesidir:

𝑑
(
𝑥
,
𝑦
)
=
∑
𝑖
=
1
𝑛
(
𝑥
𝑖
−
𝑦
𝑖
)
2
d(x,y)= 
i=1
∑
n
​
 (x 
i
​
 −y 
i
​
 ) 
2
 
​
 
Ancak, Manhattan mesafesi ve Minkowski mesafesi gibi diğer ölçümler de kullanılabilir.

Komşuların Seçimi: Hesaplanan mesafeler sıralanır ve en küçük mesafeye sahip 
𝐾
K komşu seçilir. Bu komşuların sınıfları veya değerleri, yeni veri noktasının tahmininde kullanılır.

Tahmin Yapma:

Sınıflandırma İçin: Seçilen 
𝐾
K komşunun sınıflarına bakılır ve en çok tekrarlanan sınıf yeni veri noktasının sınıfı olarak atanır (çoğunluk oyu yöntemi).
