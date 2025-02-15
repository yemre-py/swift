# 1. Temeller

## 1.1 Constants and Variables

Swift'te deðiþkenleri `let` ve `var` anahtar kelimeleriyle tanýmlarýz. `let` ile tanýmlanan deðiþkenler deðiþtirilemez sadece bir kez deðer atanabilir, `var` ile tanýmlanan deðiþkenler deðiþtirilebilir.

## 1.2 Declaring Constants and Variables

Sabitler ve deðiþkenler kullanýlmadan önce mutlaka tanýmlanmalýdýr. Sabitler için `let`, deðiþkenler için `var` anahtar kelimelerini kullanýlýr. Aþaðýda örnek tanýmlamalarý görebilirsin:

```swift
let maxNumberOfLoginAttempts = 10
var currentLoginAttempt = 0
```

Bu kod þöyle okunur:

```plaintext
maxNumberOfLoginAttempts adýnda bir sabit tanýmladýk ve deðeri 10'a eþitledik.
currentLoginAttempt adýnda bir deðiþken tanýmladýk ve baþlangýç deðerini 0'a eþitledik.
```

Bu örnekte, `maxNumberOfLoginAttempts` sabit olarak tanýmladýk. Çünkü maksimum giriþ deneme sayýsý deðiþtirilmeyecek. `currentLoginAttempt` deðiþkeni ise her giriþ denemesi sonrasý artacak.

Eðer deðeri kodda hiç deðiþtirilmeyecekse sabit olarak tanýmlamak daha mantýklýdýr. Aksi takdirde deðiþken olarak tanýmlamak daha mantýklýdýr.

Sabit deðer tanýmlarken, yukarýdaki örnekte olduðu gibi bir baþlangýç deðeri verebilirsin. Alternatif olarak, bu deðeri sonradan da verebilirsin.

```swift
var surface = "moon"
let gravity: Float
// gravity deðiþkenine halen deðer atanmamýþ.

if surface == "earth" {
    gravity = 9.81
} else {
    gravity = 1.62
}
// þuan gravity deðiþkenine deðer atandý ve okunabilir hale geldi.
```

Bu kod þöyle okunur:

```plaintext

```
