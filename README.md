# Lcd-
// nama  : Deni Efendi 
// kelas. : D3 TME 4C 


#include <Wire.h>
#include <LiquidCrystal_I2C.h>

// Set the LCD address to 0x29 for a colum chars and row line display
LiquidCrystal_I2C lcd(0x27, 16, 2);

void setup() {
  // Initialize the LCD
  lcd.begin();
  
  // Turn on the backlight
  lcd.backlight();
  
  // Print a message to the LCD
  lcd.setCursor(0, 0); // Set the cursor to column 0, line 1
  lcd.print("Hello, World!");
  
  lcd.setCursor(0, 1); // Set the cursor to column 0, line 2
  lcd.print("Arduino LCD I2C");
}

void loop() {
  // No need to repeat anything
}
