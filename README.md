# RGB LED controlling with Android Things on Raspberry Pi 3

## Describe
 + Using three pins to control an RGB LED displaying in different colors.
 + Get input from a button and then change the pace of color displaying (ex 1). For example, the RGB LED changes colors in 2s by default. After a button is pressed, the rate will change to 1s, then 0.5s, 0.1s and back to 2s. 
 + Similar to exercise 1, control the RGB LED by using PWM to change the brightness of the led. Please read this link for more details of PWM
 + Get input from a button and change the brightness of each color of the RGB LED. For example, the RGB LED changes the brightness of red, green, blue by default. After a button is pressed, only the red one is changing its brightness, then green, blue and back to three colors.
+ Blink each LED in different paces. The RED LED is blinking every 0.5s, the green is 2s, and the blue is 3s.

## GPIO ports

| Peripherals    |  Raspberry Pi 3 ports |
|----------------|-----------------------|
| LED RED        |  BCM2|
| LED GREEN      |  BCM3|
| LED BLUE       |  BCM4|
| COMMUM CATOT   |  GND|
| COMMUM ANOT    |  5V|
| BUTTON         |  BCM20|
| PWM PIN        |  PWM0|

## Usage
+ At the exercise 3, add this line: `import com.google.android.things.pio.Pwm` into the MainActivity.java
+ To use the pio-softpwm driver at the exercise 4, simply add the line below to build.gradle: `implementation com.leinardi.android.things:pio-softpwm:0.2` and add `import com.leinardi.android.things.pio.SoftPwm` into the MainActivity.java
## MEMBERS

+ Trần Minh Đức - 1610800
+ Trần Thanh Sang - 1612939
+ Nguyễn Minh Nhựt - 1612483
+ Lê Đức Trung - 1613786
