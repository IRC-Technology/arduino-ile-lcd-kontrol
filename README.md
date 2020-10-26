#include <LiquidCrystal.h> //LCD'nin kütüphanesidir. NOT: GLCD VE OLED EKRANLARININ KÜTÜPHANESİ FARKLIDIR!!

LiquidCrystal lcd(12, 11, 5, 4, 3, 2); //LCD pinlerinin bağlantısını temsil eder.

void setup() {
  
lcd.begin(16, 2);   //Ekranımızın özelliğini temsil eder (16 sütun sayısını, 2 ise satır sayısını)

lcd.setCursor(1, 0);  //İlk değer soldan bırakılacak boşluğu temsil eder.
                      //İkinci değer satırı temsil eder. 0 değeri aslında birinci satırı temsil eder,
                      // 1 değeri ise ikinci satırı temsil eder.

lcd.print("IRC Technology"); //Yazacağınız kelime veya cümle yazılır. TÜRKÇE KARAKTER KULLANMAYIN!!

lcd.setCursor(4, 1);  //İlk değer soldan bırakılacak boşluğu temsil eder.
                      //İkinci değer satırı temsil eder. 0 değeri aslında birinci satırı temsil eder,
                      // 1 değeri ise ikinci satırı temsil eder.

lcd.print("ABONE OL"); //Yazacağınız kelime veya cümle yazılır. TÜRKÇE KARAKTER KULLANMAYIN!!

}

void loop() {

}
