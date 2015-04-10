#include <LiquidCrystal.h> //Ekran kütüphanesini taslağa dahil ettik.
LiquidCrystal lcd(12,11,5,4,3,2);
int sicaklik =0; //Sıcaklık değişkenimiz.
const int sicaklik_pin= A0; //LM35'i bağladığımız pin.

void setup() {
lcd.begin(16,2);
}

void loop() {
lcd.clear();
sicaklik = analogRead(sicaklik_pin); //Ham analog veriyi değişkenimizde sakladık.
sicaklik = sicaklik * 0.48828125; //Celcius cinsinden sıcaklık birimine dönüştürdük.
lcd.print("Sicaklik: "); // Bilgileri
lcd.print(sicaklik); // ekrana
lcd.print("C"); // yazdırdık...
delay(1000);
}
