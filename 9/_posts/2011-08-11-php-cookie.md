---
layout: post
title: php cookies
---
Cookie(çerez), gerektiğinde kullanılması için client tarafından
oluşturulan  dosyadır. Oluşturduğumuz bu dosya içinde kullanıcı bilgileri, kullanıcının tercihleri gibi tanımlayıcı bilgiler saklayabiliriz. Cookieler HTML kod içine gömülüdür ve server-client arasinda gidip gelirler. Client'imiz web tarayıcımızdır. Server ise web sayfasının bulunduğu makinede çalışan programdır. Cookieler kişiye özel web sayfası yapmak, biz internette gezinirken veri kaydetmek, istatistik tutmak gibi işlerde kullanılır. Örneğin, sitemizde birkaç çeşit tema kullanıyorsak, bu temaları cookiede tutulan tek bir değer ile değiştirebiliriz. Cookieler ile ilgili yapılan temel işlemler; Oluşturma, değer atama, değer okuma, değerini değiştirme ve silme şeklindedir.

####cookie oluşturma

Cookie oluşturmak için `setcookie` fonksiyonu kullanmalıyız. Bu fonksiyonun parametreleri sırasıyla **değişken, değer,
geçerlilik süresi** dir;

<script src="https://gist.github.com/1139640.js"> </script>

---

Cookienin geçerlilik süresini bir başka bir şekilde ayarlayabiliriz;

<script src="https://gist.github.com/d3a46d835ca51958858e.js"> </script>

####cookie'ye değer atama

Php'de, `$_COOKIE` değişkenini, bir cookie değerini atamak için
kullanabiliriz. Aşağıda, **"user"** adlı cookienin değerini alıp ve bir
sayfada görüntüleyen örnek paylaştım;

<script src="https://gist.github.com/9bf3d9a95f115910e996.js"> </script>

---

Aşağıdaki örnekteki gibi bir cookie olup olmadığını öğrenmek için `isset()` işlevini
kullanabiliriz;

<script src="https://gist.github.com/4de29c6a6a09cc5b30a3.js"> </script>

####cookie silme

Cookie silmek için yine `setcookie` fonsiyonunu kullanmamız gerekli. **"user"**
değişkenine boş değer atayarak ve geçerlilik süresini şimdiki zamandan daha önce
bir zaman olacak şekilde ayarlayarak oluşturduğumuz cookienin geçerliliğini
yitirmiş oluyoruz;

<script src="https://gist.github.com/a3badd41586322d8cb05.js"> </script>

