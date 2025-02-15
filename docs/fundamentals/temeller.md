# 1. Temeller

## 1.1 Constants and Variables

Swift'te de�i�kenleri `let` ve `var` anahtar kelimeleriyle tan�mlar�z. `let` ile tan�mlanan de�i�kenler de�i�tirilemez sadece bir kez de�er atanabilir, `var` ile tan�mlanan de�i�kenler de�i�tirilebilir.

## 1.2 Declaring Constants and Variables

Daimiler ve de�i�kenler kullan�lmadan �nce mutlaka tan�mlanmal�d�r. Daimiler i�in `let`, de�i�kenler i�in `var` anahtar kelimelerini kullan�l�r. A�a��da �rnek tan�mlamalar� g�rebilirsin:

```swift
let maxNumberOfLoginAttempts = 10
var currentLoginAttempt = 0
```

Bu kod ��yle okunur:

```plaintext
maxNumberOfLoginAttempts ad�nda bir Daimi tan�mlad�k ve de�eri 10'a e�itledik.
currentLoginAttempt ad�nda bir de�i�ken tan�mlad�k ve ba�lang�� de�erini 0'a e�itledik.
```

Bu �rnekte, `maxNumberOfLoginAttempts` Daimi olarak tan�mlad�k. ��nk� maksimum giri� deneme say�s� de�i�tirilmeyecek. `currentLoginAttempt` de�i�keni ise her giri� denemesi sonras� artacak.

E�er de�eri kodda hi� de�i�tirilmeyecekse Daimi olarak tan�mlamak daha mant�kl�d�r. Aksi takdirde de�i�ken olarak tan�mlamak daha mant�kl�d�r.

Daimi de�er tan�mlarken, yukar�daki �rnekte oldu�u gibi bir ba�lang�� de�eri verebilirsin. Alternatif olarak, bu de�eri sonradan da verebilirsin.

```swift
var surface = "moon"
let gravity: Float
// gravity de�i�kenine halen de�er atanmam��.

if surface == "earth" {
    gravity = 9.81
} else if surface == "mars" {
    gravity = 3.71
} else {
    gravity = 1.62
}
// �uan gravity de�i�kenine de�er atand� ve okunabilir hale geldi.
```

Bu �rnekte, gravity de�i�keni bir Daimitir ve surface de�i�kenine ba��ml�d�r. `if` ko�ulu ile gravity de�i�kenine daimi bir de�er atan�r.

Tek sat�rda birden fazla de�i�ken tan�mlanabilir.

```swift
let red = 0, blue = 0, green = 0
```

## 1.3 Type Annotations

Daimi ve de�i�kenlerin hangi tipte oldu�unu belirtmek i�in `type annotation` kullan�l�r. Daiminin ya da de�i�kenin ad�n�n ard�ndan `:` i�areti ve tipi yaz�l�r.

```swift
var welcomeMessage: String
```

```plaintext
T�r� String olan welcomeMessage ad�nda bir de�i�ken tan�mla.
```

Tek sat�rda birden fazla de�i�keni ayn� �ekilde tan�mlayabilirsin.

```swift
var red, blue, green: Float
```

## 1.4 Naming Constants and Variables

De�i�ken ve daimiler neredeyse her karakteri i�erebilir, UNICODE karakterler de buraya dahildir.

```swift
let ? = 3.14159
let ?? = "????"
let ???? = "dogcow"
```

Daimiler ve de�i�kenlerin isimleri

- bo�luk i�eremez
- matematiksel semboller i�eremez
- oklar i�eremez
- g�izli Unicode karakterler i�eremez
- �izgi ya da kutu-�izgiler i�eremez
- say� ile ba�layamaz

Bir t�rde bir de�i�ken tan�mlad�ktan sonra, ayn� isimde ba�ka bir de�i�ken tan�mlayamazs�n veya farkl� bir t�rde ba�ka bir de�i�ken tan�mlayamazs�n. Bir daimiyi de�i�kene, de�i�keni daimiye �eviremezsin.

> **Not**
>
> E�er Swift'te keyword olarak kullan�lan bir isim kullanmak istersen, isminizi `backticks` i�ine al�n.
>
> ```swift
> let `if` = "if"
> ```

De�i�kenlerin de�erini ba�lang�� tipine uygun olarak de�i�tirebilirsin.

```swift
var friendlyWelcome = "Hello!"
friendlyWelcome = "Bonjour!"
// friendlyWelcome art�k "Bonjour!" de�erini ta��r.
```

Daimilerin de�erini de�i�tiremezsin.

```swift
let languageName = "Swift"
languageName = "Swift++"
// Cannot assign to value: 'language' is a 'let' constant
```

## 1.5 Printing Constants and Variables

Daimiler ve de�i�kenlerin de�erini ekrana yazd�rmak i�in `print(_:separator:terminator:)` fonksiyonunu kullan�r�z.

```swift
print(friendlyWelcome)
```
