# 2. Hafta

Koç Okulu FRC Kulübünün ikinci toplantısına hoşgeldiniz. Bu yönergede, size dağıtılacak malzemeler ile Arduino üzerinde LED Blink Devresi yapacağız.

LED Blink Devresi, Arduino üzerindeki ledlerin sürekli olarak açılıp kapanmasını sağlayan devredir.

## Adım 1  → Parçaları Tanıyalım

![Arduino UNO](https://slabstatic.com/prod/uploads/ldjloyi2/posts/images/MbO6bwTa4m67S3l0s455gcCy.png)

![Breadboard](https://slabstatic.com/prod/uploads/ldjloyi2/posts/images/5H1zRYJdu2-bRuVEViyhCwbe.png)

Uno, Arduino kartları arasında en popüler olandır. Akıllı sistemlerde kullanımı uygun olduğu için tercih edilir.









![LED](https://slabstatic.com/prod/uploads/ldjloyi2/posts/images/EVo2xPjBO84YMWW07wTUXaJe.png)

Breadboard, elektronik devre geliştirmek ve test etmek için kullanılan lehimsiz inşa taşı.





Terminallerinden geçen elektrik sonucu ışık yayan elektronik cihaz.







![Direnç](https://slabstatic.com/prod/uploads/ldjloyi2/posts/images/UXmcqYKB79Pvwpuhbq0QJRrE.png)





Elektrik akışına karşı direnç sağlayan alet.

## Adım 2 → Devreyi Kurun

Aşağıdaki devreyi breadboard üzerinde kurun. Kabloların rengine dikkat etmenize gerek olmadığını hatırlatırız.

![](https://slabstatic.com/prod/uploads/ldjloyi2/posts/images/kLbAin-VOfw6I_F4sUmsjb7H.jpeg)

## Adım 3 → Kodu Yapıştırın

Arduino IDE'yi açın, yeni bir proje oluşturun ve aşağıdaki kodu yapıştırın. Arduino'yu bilgisayarınıza bağladıktan sonra sol üstteki ok işareti ile kodu Arduino'ya gönderin.

```C++
#define LED_PIN 12

void setup() {
  // initialize digital pin LED_PIN as an output.
  pinMode(LED_PIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_PIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(1000);                       // wait for a second
  digitalWrite(LED_PIN, LOW);    // turn the LED off by making the voltage LOW
  delay(1000);                       // wait for a second
}
```

## Bitiş

Bu kodu çalıştırmanız ardından LED, 1 saniye yanıp 1 saniye sönecektir.
