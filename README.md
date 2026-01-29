# TestingMachine

Firmware for a standalone quiz/test device with voice prompts, LCD output, keypad input, and optional thermal printing. Questions, answers, and audio files are stored on an SD card, and the device guides the user through a test session with immediate feedback.

![Photo](images/2.png)

Video: https://youtu.be/E8pNuMWTcd8

## Repository Description (About)
Firmware for a quiz/test device that loads questions and audio from SD, plays voice prompts, reads keypad input, and prints results.

## How It Works
- Questions and answers are loaded from SD card files.
- Audio prompts are played via DFPlayer Mini (MP3 folders).
- The user enters answers with hardware buttons.
- The LCD shows questions, answers, and progress.
- Results can be printed on a thermal printer (optional).

## Hardware Modules (from code)
- DFPlayer Mini for MP3 playback
- LCD with I2C backpack (16x2)
- SD card module
- Thermal printer (optional)
- Button matrix / analog button input

## Files & Media
- `mp3/` — audio prompts per folder
- `Q.txt`, `A.txt`, `S.txt` — question/answer metadata
- `tale/` — additional audio content

## Build Notes
- PlatformIO project (`platformio.ini` included).
- Uses ArduinoJson, DFPlayerMini_Fast, LiquidCrystal_I2C, SD, and Adafruit_Thermal libraries.

## Hashtags
#Firmware #QuizDevice #DFPlayer #SDCard #Arduino #Embedded #AudioPrompt #ThermalPrinter