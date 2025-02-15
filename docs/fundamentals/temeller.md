# 1. Temeller

## 1.1 Constants and Variables

Swift'te de�i�kenleri `let` ve `var` anahtar kelimeleriyle tan�mlar�z. `let` ile tan�mlanan de�i�kenler de�i�tirilemez sadece bir kez de�er atanabilir, `var` ile tan�mlanan de�i�kenler de�i�tirilebilir.

## 1.2 Declaring Constants and Variables

Sabitler ve de�i�kenler kullan�lmadan �nce mutlaka tan�mlanmal�d�r. Sabitler i�in `let`, de�i�kenler i�in `var` anahtar kelimelerini kullan�l�r. A�a��da �rnek tan�mlamalar� g�rebilirsin:

```swift
let maxNumberOfLoginAttempts = 10
var currentLoginAttempt = 0
```

Bu kod ��yle okunur:

```plaintext
maxNumberOfLoginAttempts ad�nda bir sabit tan�mlad�k ve de�eri 10'a e�itledik.
currentLoginAttempt ad�nda bir de�i�ken tan�mlad�k ve ba�lang�� de�erini 0'a e�itledik.
```

Bu �rnekte, `maxNumberOfLoginAttempts` sabit olarak tan�mlad�k. ��nk� maksimum giri� deneme say�s� de�i�tirilmeyecek. `currentLoginAttempt` de�i�keni ise her giri� denemesi sonras� artacak.

E�er de�eri kodda hi� de�i�tirilmeyecekse sabit olarak tan�mlamak daha mant�kl�d�r. Aksi takdirde de�i�ken olarak tan�mlamak daha mant�kl�d�r.

Sabit de�er tan�mlarken, yukar�daki �rnekte oldu�u gibi bir ba�lang�� de�eri verebilirsin. Alternatif olarak, bu de�eri sonradan da verebilirsin.

```swift
var surface = "moon"
let gravity: Float
// gravity de�i�kenine halen de�er atanmam��.

if surface == "earth" {
    gravity = 9.81
} else {
    gravity = 1.62
}
// �uan gravity de�i�kenine de�er atand� ve okunabilir hale geldi.
```

Bu kod ��yle okunur:

```plaintext

```
