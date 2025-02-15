# 1. Temeller

## 1.1 Constants and Variables

Swift'te deðiþkenleri `let` ve `var` anahtar kelimeleriyle tanýmlarýz. `let` ile tanýmlanan deðiþkenler deðiþtirilemez sadece bir kez deðer atanabilir, `var` ile tanýmlanan deðiþkenler deðiþtirilebilir.

## 1.2 Declaring Constants and Variables

Daimiler ve deðiþkenler kullanýlmadan önce mutlaka tanýmlanmalýdýr. Daimiler için `let`, deðiþkenler için `var` anahtar kelimelerini kullanýlýr. Aþaðýda örnek tanýmlamalarý görebilirsin:

```swift
let maxNumberOfLoginAttempts = 10
var currentLoginAttempt = 0
```

Bu kod þöyle okunur:

```plaintext
maxNumberOfLoginAttempts adýnda bir Daimi tanýmladýk ve deðeri 10'a eþitledik.
currentLoginAttempt adýnda bir deðiþken tanýmladýk ve baþlangýç deðerini 0'a eþitledik.
```

Bu örnekte, `maxNumberOfLoginAttempts` Daimi olarak tanýmladýk. Çünkü maksimum giriþ deneme sayýsý deðiþtirilmeyecek. `currentLoginAttempt` deðiþkeni ise her giriþ denemesi sonrasý artacak.

Eðer deðeri kodda hiç deðiþtirilmeyecekse Daimi olarak tanýmlamak daha mantýklýdýr. Aksi takdirde deðiþken olarak tanýmlamak daha mantýklýdýr.

Daimi deðer tanýmlarken, yukarýdaki örnekte olduðu gibi bir baþlangýç deðeri verebilirsin. Alternatif olarak, bu deðeri sonradan da verebilirsin.

```swift
var surface = "moon"
let gravity: Float
// gravity deðiþkenine halen deðer atanmamýþ.

if surface == "earth" {
    gravity = 9.81
} else if surface == "mars" {
    gravity = 3.71
} else {
    gravity = 1.62
}
// þuan gravity deðiþkenine deðer atandý ve okunabilir hale geldi.
```

Bu örnekte, gravity deðiþkeni bir Daimitir ve surface deðiþkenine baðýmlýdýr. `if` koþulu ile gravity deðiþkenine daimi bir deðer atanýr.

Tek satýrda birden fazla deðiþken tanýmlanabilir.

```swift
let red = 0, blue = 0, green = 0
```

## 1.3 Type Annotations

Daimi ve deðiþkenlerin hangi tipte olduðunu belirtmek için `type annotation` kullanýlýr. Daiminin ya da deðiþkenin adýnýn ardýndan `:` iþareti ve tipi yazýlýr.

```swift
var welcomeMessage: String
```

```plaintext
Türü String olan welcomeMessage adýnda bir deðiþken tanýmla.
```

Tek satýrda birden fazla deðiþkeni ayný þekilde tanýmlayabilirsin.

```swift
var red, blue, green: Float
```

## 1.4 Naming Constants and Variables

Deðiþken ve daimiler neredeyse her karakteri içerebilir, UNICODE karakterler de buraya dahildir.

```swift
let ? = 3.14159
let ?? = "????"
let ???? = "dogcow"
```

Daimiler ve deðiþkenlerin isimleri

- boþluk içeremez
- matematiksel semboller içeremez
- oklar içeremez
- güizli Unicode karakterler içeremez
- çizgi ya da kutu-çizgiler içeremez
- sayý ile baþlayamaz

Bir türde bir deðiþken tanýmladýktan sonra, ayný isimde baþka bir deðiþken tanýmlayamazsýn veya farklý bir türde baþka bir deðiþken tanýmlayamazsýn. Bir daimiyi deðiþkene, deðiþkeni daimiye çeviremezsin.

> **Not**
>
> Eðer Swift'te keyword olarak kullanýlan bir isim kullanmak istersen, isminizi `backticks` içine alýn.
>
> ```swift
> let `if` = "if"
> ```

Deðiþkenlerin deðerini baþlangýç tipine uygun olarak deðiþtirebilirsin.

```swift
var friendlyWelcome = "Hello!"
friendlyWelcome = "Bonjour!"
// friendlyWelcome artýk "Bonjour!" deðerini taþýr.
```

Daimilerin deðerini deðiþtiremezsin.

```swift
let languageName = "Swift"
languageName = "Swift++"
// Cannot assign to value: 'language' is a 'let' constant
```

## 1.5 Printing Constants and Variables

Daimiler ve deðiþkenlerin deðerini ekrana yazdýrmak için `print(_:separator:terminator:)` fonksiyonunu kullanýrýz.

```swift
print(friendlyWelcome)
```
