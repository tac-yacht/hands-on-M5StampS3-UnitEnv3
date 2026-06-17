# 2: LチカでStampS3の動作とMicroPythonでの制御方法を理解する

この章では、最初の動作確認として LED を点滅させます。

## 想定時間

5 分

## この章のゴール

- Thonny から StampS3 にコードを書き込む
- 最小コードで LEDを点滅(Lチカ)させ、StampS3を内蔵のMicro Pythonで制御できることを確認する

## 手順

StampS3に内蔵されたLEDを、pythonから点滅させてみましょう。
StampS3には、RGB LEDが搭載されています。

![LEDの位置](image/led_position.png)

以下のソースコードを貼り付け、実行してみましょう。

```python
from machine import Pin
from neopixel import NeoPixel
from time import sleep

Pin(38, Pin.OUT).value(1)
led = NeoPixel(Pin(21), 1)

while True:
    led[0] = (0,255,0)
    led.write()
    sleep(0.25)

    led[0] = (0,0,0)
    led.write()
    sleep(0.75)
```

LED1が0.25秒点灯し、0.75秒消灯する動作を繰り返すはずです。

応用として、LEDの色を変えて点滅させてみましょう。4行目の`"(0,255,0)"`を`"(255,0,0)"`に変更してみてください。

このように、そのほかのMicroPythonを入れたボードと同様に、MicroPythonから`Pin()` 関数を使うことで、GPIOの操作が簡単に行えます。

---
- 次: [3: SIM の開通と SORACOM Harvest Data の設定](../chapter3/README.md)
- 前: [1: 環境構築 (Thonny インストール)](../chapter1/README.md)
