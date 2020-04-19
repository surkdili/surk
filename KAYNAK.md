# Değişkenler
Değişken isimleri harf ile başlamak zorundadır. 
Türkçe karakter içerebilir.
Tipler; 
1. Sayı
2. Küsüratlı Sayı
3. Metin
4. Mantıksal 

```python
isim = "Bu bir metin değeridir."
İSİM = "Bu da bir metin."
isim_soyisim = "Snakecase kullanabilirsiniz."
isimSoyisim = "Camelcase kullanabilirsiniz."
isim12Soyisim21 = "Değişken isminde sayı bulanabilir."
sayı = 19
noktalıSayı = 19.99
çokUzunBirSayı = 9999999999.99999999999
mantıksalBirİfade = doğru
diğerÖrnek = yanlış
```

# Mantıksal Kontroller

```python
isim = "ahmet"
yaş = 17
mantıksalİfade = yanlış
küçükSayı = -10
çokKüçükSayı = -999

eğer isim == "ahmet" ise:
	yaz("Kullanıcı ismi Ahmet'miş.")
değilse:
	yaz("Kullanıcı ismi Ahmet değilmiş.")


eğer yaş >= 18 ise:
	yaz("Kullanıcı reşit değil. Yaşı 18'in altında.")
değilse:
	yaz("Kullanıcı reşit. Yaşı 18 veya üstü.")

eğer küçükSayı < 0 ise:
	yaz("Sayı negatif.")

eğer küçükSayı > 0 ise:
	yaz("Say pozitif.")
```

# Döngüler

```python
sayı = 10
sayı > 0 olduğu sürece: 
	yaz("sayı değeri : " , sayı)
	sayı = sayı - 1
yaz("döngü bitti. sayı artık : " , sayı)
```

# Operatörler
Tüm basit oepratörler diğer dillerde olduğu gibi çalışmakta.

```python
sayı1 = 10 + 20 # sayı 30 oldu.
sayı2 = sayı1 + 11 # sayı2 = 41 oldu. 
sayı3 = sayı1 + sayı1 # sayı3 değeri 71 oldu. 

sayı4 = sayı1 * sayı2
sayı5 = sayı1 + sayı2 * sayı3 / 10
sayı6 = (sayı1 + sayı2) * sayı3 / 10

isim = "Ahmet"
soyisim = "Yılmaz"
yaş = 21

tamİsim = isim + " " + soyisim # Ahmet Yılmaz
tanım = isim + " " + " " + " isimli kullanıcı " + metin(yaş) + " yaşındadır."
```

# Uçbirim Veri Akışları

Yapılan ver girişlerin metin(string) türünde okunur. Sayı girişlerini sayı tipini çevirmek gereklidir.
```python
girilenYazı = oku("Lütfen metni yazıp enter'a basınız.")
yaz(girilenYazı)
yaz("Girdiğiniz metin: " , girilenYazı)

sayı1 = oku("ilk sayı : ") # 15 giriniz.
sayı2 = oku("ikinci sayı : ") # 20 giriniz.

yaz("Tür çevri işleminden önce yapılan toplam işleminin sonucu : " , sayı1 + sayı2 ) # 1520 yazacaktır. Değişken türlerinden en az biri metin türü olduğu için + operatörü metin türünde birleştirme yapılır.

yaz("Tür çevri işleminden sonra yapılan toplam işleminin sonucu : ", tamSayı(sayı1) + tamSayı(sayı2)) # 35 yazacaktır. İki değeri sayı türüne çevirdiğinden + operatörü matematiksel toplama yapacaktır.
```
