# --Ardunio-ile-Giris-cikis-Uygulamalari-
Ardunio Uno Geliştirme Kartı
• 9 adet buton
• 8 adet LED
• 8 adet 220Ω
• 9 adet 4.7KΩ
• 1 adet buzzer
• Ara kablo, Yan keski vb. malzemeler
Adımlar

1) İstediğiniz 8 adet pine 8 adet buton ve 8 adet 4.7 KΩ ‘luk dirençleri uygun şekilde
bağlayınız (Butona basıldığında lojik 1, basılmadığında lojik 0 olacak şekilde bağlantıları
yapabilirsiniz). Boşta kalan diğer pinlerden 8 tanesine, 8 adet LED ve 8 adet 220 Ω ‘luk
dirençleri bağlayınız. Ayrıca istediğiniz boş olan başka bir pine de 1 adet buzzer bağlayınız.
(Butonları ve LEDleri kendi aralarında grup oluşturacak şekilde sıralı bir biçimde
Breadborda yerleştiriniz ve 1-8 arası numaralandırınız.)

2) 1. Butona 3 defa basıp çekince, bütün ledlerin sönmesi ve sadece 1. LED ‘in
yanması isteniyor. 3 defa basma işleminde buton arkı oluşmaması için bekleme
süresi koyunuz. (Yukarıdaki bekleme fonksiyonuna bakınız)

3) 2. Butona 1 defa basıp çekince, bütün ledlerin sönmesi ve ledlerin (1-8 nolu ledler)
sırayla yanması isteniyor. Önce 1. Led yanacak, ardından 2. Led ile 1. Led birlikte yanacak.
Devre bu şekilde devam edecek ve sonunda bütün ledler yanık olarak kalacak. Ledlerin geçişleri
için bekleme süresi koyunuz.

4) Bir önceki basamaktaki işlemlerin tersi yapılacak. Yani 3. Butona 1 defa basıp çekince, bütün
ledlerin sönmesi ve ledlerin (8-1)) ters sırayla yanması isteniyor. Önce 8. Led yanacak, ardından
7. Led ile 8. Led birlikte yanacak. Devre bu şekilde devam edecek ve sonunda bütün ledler
yanık olarak kalacak. Ledlerin geçişleri için bekleme süresi koyunuz.

5) 4. Butona 1 defa basıp çekince, bütün ledlerin sönmesi ve ledlerin (1-8) binary olarak artacak
şekilde yanması isteniyor. Devreye binary olarak ileriye sayacaktır. Önce 1. Led yanacak
(binary 00000001  1 sayısı), ardından 1. Led sönerken 2. Led yanacak (binary 00000010 
2 sayısı), ardından 1. ve 2. Ledler birlikte yanacak (binary 00000011  3 sayısı)… Devre bu
şekilde 255 ‘e (binary 11111111) kadar sayacak ve sonunda bütün ledler yanacaktır. Ledlerin
geçişleri için bekleme süresi koyunuz.

6) 5. Butona 1 defa basıp çekince, bütün ledlerin sönmesi ve sadece tek numaralı ledlerin (1. -
3. - 5. - 7. ledlerin) aynı anda yanması ve yanık kalması isteniyor.

7) 6. Butona 1 defa basıp çekince, bütün ledlerin sönmesi ve sadece çift numaralı ledlerin (2. -
4. - 6. - 8. ledlerin) aynı anda yanması ve yanık kalması isteniyor.

8) 7. Butona 1 defa basıp çekince, bütün ledlerin sönmesi ve sadece 1. Ledin yanması, aynı
butona 2. defa basıp çekince 1. Led sönerken 2. Ledin yanması, aynı butona 3. defa basıp
çekince 2. Led sönerken 3. Ledin yanması ve devrenin bu şekilde sonuna kadar gitmesi ve tekrar
başa dönmesi isteniyor. Yani aynı butona 8. defa basıp çekince 7. Led sönerken 8. Ledin
yanması, aynı butona 9. defa basıp çekince devrenin başa dönmesi 8. Led sönerken 1. Ledin
yanması isteniyor. Buton arkı oluşmaması için bekleme süresi koyunuz.

9) 8. Butona 1 defa basıp çekince, bütün ledlerin sönmesi ve buzzer ’ın belirli bir süre (bekleme
süresi koyunuz) ses vermesi isteniyor.
