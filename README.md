Jupyter Notebook için Türkçe Markdown kullanım örnekleri.

# Markdown

Merhaba Jupyter Notebook'da Markdown satırları nasıl kullanılır özetleme çalışacağım.

## İçindekiler

[Markdown Modu](#Markdown-Modu)  
[Başlık ve Alt Başlıklar](#Başlık-ve-Alt-Başlıklar)  
[Satır ve Yazı Tipleri](#Satır-ve-Yazı-Tipleri)  
[Blok ve alıntı görünümleri](#Blok-ve-Alıntı-Görünümleri)  
[Madde işaretleri](#Madde-İşaretleri)  
[Link Ekleme](#Link-Ekleme)  
[Resim Ekleme](#Resim-Ekleme)  
[Kod Görünümü](#Kod-Görünümü)  
[Matematik Formülleri](#Matematik-Formülleri)  
[Tablo Oluşturma](#Matematik-Formülleri)  
[Uzun Çizgi](#Uzun-Çizgi)  
[Html Kodları](#Html-Kodları) 


***

### Markdown Modu
Öncelikle bu hücrelerde iki şey yapabiliriz. Kod yazabilir ya da bunun gibi açıklamalar ekleyebiliriz.  
Eğer hücreyi olarak `In [ ]:` görüyorsanız bu kod yazmak için açılmış bir hücredir.  
Hücreleri markdown moduna almak için, yukarıdaki açılır menüden 'Code' olan seçeneğini, 'Markdown' olarak değiştirmemiz gerekir.  
Klavye kısayolu için;  
`In [ ]:` yazısına tıklarsanız mavi olur. Bu da hücre dışında olduğunuzu gösterir.  
Bu durumdayken klavyede **M** tuşuna basktığınızda hücreyi markdown moduna almış olursunuz.
***

### Başlık ve Alt Başlıklar
Hücrelerin modunu değiştirdiğimizde artık açıklamalar girebiliriz. **#** karakterinden sonra bir boşluk bıraktığınızda, yazdığınız metin kalın başlık olarak görünür.  
Ne kadar çok # kullanırsanız, başlığınız alt başlık olarak küçülür.  

Kullanımı:  
`# Başlık`  
`## Alt Başlık`  
`### Küçük Alt Başlık`   



# Başlık  
## Alt Başlık  
### Küçük Alt Başlık

***

### Satır ve Yazı Tipleri 

Bir alt satıra geçmek için noktadan sonra en az iki boşluk kullanmanız gerekir.  
İki boşluk yapıp alt satıra geçtiğinizde, cümleniz bunun gibi yeni bir satır olarak görünür.  

Cümle içinde kelimeleri kalın olarak belirtmek için, kelimelenin başlangıç ve bitişinde `**` kullanırız.  
Böylece **istediğimiz kelime** kalın yazılmış olur.    
  
Tek yıldız `*`  olarak kullanırsak; *italik* yazmış oluruz.  

Üç yıldız `***` olarak kullanırsak ***hem kalın hem de italik*** olur.  

Üzeri çizili kelimeler için `~~` kullanılır. ~~Üzeri çizilmiş~~	

Kod blogu için enter üzerinde bulunan \` tırnak işareti kullanılır.  `Kod`

***

### Blok ve Alıntı Görünümleri

> `>` Büyüktür işareti ile başladığımızda blok olarak görünür.  

>> `>>` İki büyüktür işareti ile böyle

>>> `>>>` Üç büyüktür işareti ile böyle

***

### Madde İşaretleri

Satır başları;   `-` , `*` , `+`    ile başlarsa madde işareti olarak görünür.

- İstediğiniz yazıyı madde madde yazabilirsiniz.

Tab boşluğu ile alt maddeler de eklendiğinde böyle görünür.

- Madde 1
- Madde 2
    - Madde 2 alt madde
- Madde 3

Numerik olarak da 1. ile başlayan maddeler ekleyebiliriz.

1. Birinci satır
2. İkinci satır
3. Üçüncü satır

Numerik satırların içerisinde tab boşluğunu kullanarak alt maddeler de eklenebilir.

1. Birinci satır
2. İkinci satır
    1. İkinci satırın ilk maddesi
    2. ikinci satırın ikinci maddesi
3. Üçüncü satır

Görev listeleri için `-` işaretinden sonra köşeli parantezler `[ ]` ve `[x]` kullanılır.

- [ ] Devam ediyor
- [x] Tamamlandı

***

### Link Ekleme

Köşeli parantez içine yazılan kelime, tıklanılacak kelime olarak görünür. Gidilecek link normal parantez içinde yanına yazılır.  
`[Tıklanılacak kelime](gidilecek site)`  


Örnek olarak [Google](https://google.com) diyelim.

Eğer aynı Jupyter Notebook saydasında maddeye link vermek istersek;  
`[Tıklanılacak kelime](#Gidilecek-Başlık)`  
(boşluk için - kullanılır)


Örnek  
(Uygulama için mecburen bir önceki maddeye gideceğiz)  
[Madde işaretleri](#Madde-işaretleri)

Siteye doğrudan link vermek istersek linki yazmamız yeterli. Mail için büyük küçük işaretleri arasına yazmamız `<isim@mail.com>` gerekir.   
www.google.com  
<isim@mail.com>

***

### Resim Ekleme

Link eklemeyle gibidir. Sadece başında ! işareti vardır.  
`![Açıklama](resimin linki "mouse üzerine gelince yazacak yazı")`  


![Google](https://www.google.com.tr/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png "Google Logosu")


Eğer resime de link vermek istersek  
`[![Açıklama](resim linki "mouse üzerine gelince yazacak yazı")](gidilecek link)`

[![Google](https://www.google.com.tr/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png "Google sitesine gider")
](https://google.com)


(link verilen hücreyi düzenlemek için hücrenin solundaki beyaz alana çift tıklanır.)

***

### Kod Görünümü

Eğer yazdığımız bir açıklamayı editörde yazılmış gibi renkli kodlar olarak görmek istersek  

\`\`\`python  

kod  

\`\`\` 

bu blogun içine kodumuzu yazabiliriz. (Kullanılan kesme işareti Enter tuşunun yanında bulunur.)

Örnek

```python
x = markdown
print(x)


def fonksiyon_ismi()
    deneme = x * y

```

***

 ### Matematik Formülleri
 
 Matematik formülleri `$formül$` şekilde yazdılığında Latex notasyon görünümü alır. Eğe iki `$$` sembolü kullanılırsa formül ortada görünür.
 
 $y = x^2$  
 ***
 $$y = x^2$$  
 ***
 $$f(x) = x^2 - x^{1 \over \pi}$$
 
 ***
 

### Tablo Oluşturma
Karakter kullanılarak bir dataframe göstermek istersek aşağıdaki gibi bir kullanımı vardır.   

Yazım   
`
| Tablo | Kolon | Son kolon |
|-------|:-----:|----------:|
| hücre | hücre | hücre     |
| hücre | hücre | hücre     |
| hücre | hücre | hücre     |
| hücre | hücre | hücre     |
`   
***


Görünüm  

| Tablo | Kolon | Son kolon |
|-------|:-----:|----------:|
| hücre | hücre | hücre     |
| hücre | hücre | hücre     |
| hücre | hücre | hücre     |
| hücre | hücre | hücre     |

***

### Uzun Çizgi

Hücreler arasında uzun ayıraç olarak uzun bir çizgi eklemek istediğimizde, hücrede `---` ya da `***` şekilde kullanabiliriz. Şu an aşağıda görmüş olduğunuz uzun çizgi oluşur.

***

### Html Kodları

Html kodlarını sayfa üzerinde kullanabiliriz.  


Yazdığımız kelimeyi <font color='red'>renkli</font> gösterebilir

<span style="font-family:Comic Sans MS">Font tipini değiştirebiliriz</span>

<div class="alert alert-info">
  <strong>Mavi</strong>
</div>

<div class="alert alert-warning">
  <strong>Sarı</strong>
</div>

<div class="alert alert-success">
  <strong>Yeşil</strong>
</div>

<div class="alert alert-danger">
  <strong>Kırmızı uyarı kutuları yapabilir</strong>
</div>

<code style="background:yellow;color:black">Önemli yerlerin üzerini marker ile çizebilir</code>  
Sadece bir <mark>kelimeyi</mark> vurgularız

<p style="background:black">
<code style="background:black;color:white">Belki de bir terminal görünümü veririz
</code>
</p>
