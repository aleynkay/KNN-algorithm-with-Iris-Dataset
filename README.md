# K-Nearest Neighbors (KNN) Algoritması

## Özet
K-Nearest Neighbors (KNN), hem sınıflandırma hem de regresyon problemlerinde kullanılabilen, gözetimli bir makine öğrenme algoritmasıdır. Temel prensibi, yeni bir veri noktasının sınıfını veya değerini, eğitim veri kümesindeki en yakın \( K \) komşusunun sınıflarına veya değerlerine bakarak tahmin etmektir.

## Temel Prensipler
1. **Mesafe Ölçümü**: Yeni bir veri noktasının eğitim verisindeki diğer veri noktalarına olan mesafesi hesaplanır. En yaygın kullanılan mesafe ölçümü Öklidyen mesafesidir:
   \[
   d(x, y) = \sqrt{\sum_{i=1}^{n} (x_i - y_i)^2}
   \]
   Ancak, Manhattan mesafesi ve Minkowski mesafesi gibi diğer ölçümler de kullanılabilir.

2. **Komşuların Seçimi**: Hesaplanan mesafeler sıralanır ve en küçük mesafeye sahip \( K \) komşu seçilir.

3. **Tahmin Yapma**:
   - **Sınıflandırma**: Seçilen \( K \) komşunun sınıflarına bakılır ve en çok tekrarlanan sınıf yeni veri noktasının sınıfı olarak atanır (çoğunluk oyu yöntemi).

## Adımlar
1. **Eğitim Verisinin Saklanması**: KNN algoritması, eğitim verisini saklar ve bu veriyi tahmin işlemi sırasında kullanır.
2. **Mesafe Hesaplama**: Yeni bir veri noktası geldiğinde, eğitim verisindeki her bir nokta ile olan mesafesi hesaplanır.
3. **Komşuların Seçimi**: Hesaplanan mesafeler sıralanır ve en küçük mesafeye sahip \( K \) komşu seçilir.
4. **Tahmin**: Seçilen komşuların sınıflarına veya değerlerine bakılarak tahmin yapılır.
