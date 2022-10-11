# workshop-music-3
YBoost workshop #3 | 12/10/2022

# MP3 Player IOT

## Objectif

You have to create a MP3 player with an arduino and an UART Serial MP3 Music Player Module.
Your MP3 player will be able to :
* Play music by pressing a button
* Change the music by pressing buttons
* Stop the music by pressing a button
* Change the volume with a rotary encoder

## Documentation 
* [How to use the serial MP3 Player module](https://www.theamplituhedron.com/articles/How-to-use-the-Serial-MP3-Player-UART-with-Speaker-by-OPEN-SMART-with-Arduino/)
* [Serial MP3 Player module official documentation](https://static1.squarespace.com/static/584d41b3f5e2310b396cd953/t/5c7c2f29104c7b336a2f8380/1551642412037/Serial+MP3+Player+A+v1.0+Manual.pdf)
* [How to use a rotary encoder](https://www.aranacorp.com/fr/utilisation-dun-encodeur-rotatif-avec-arduino/)
* [Arduino documentation : Serial](https://www.arduino.cc/reference/en/language/functions/communication/serial/)
* [Arduino documentation : Define](https://www.arduino.cc/reference/en/language/structure/further-syntax/define/)
* [Arduino documentation : Arduino Pin](https://icircuit.net/wp-content/uploads/2014/09/Arduino-uno.png)


## Step 1 : Module connection
First, you had to connect your module together and verify that it works. Here is the connection scheme :
![MP3 Player connection scheme](https://i.imgur.com/bbYFiOr.png)


## Step 2 : Configure the MP3 player module
You have to configure the module to be able to play music.
To do that, you need to setup the micro SD card by creating **folders "01" and "02"** and put your music with the name **"001xxx.mp3", "002xxx.mp3"** etc.. in it.
Follow the [official serial mp3 documentation](https://static1.squarespace.com/static/584d41b3f5e2310b396cd953/t/5c7c2f29104c7b336a2f8380/1551642412037/Serial+MP3+Player+A+v1.0+Manual.pdf) or [this page](https://www.theamplituhedron.com/articles/How-to-use-the-Serial-MP3-Player-UART-with-Speaker-by-OPEN-SMART-with-Arduino/) to configure the module.

Note that you can test the module by sending command to it with the [sscom32 serial tool](https://drive.google.com/file/d/1LE3dZDEQ341c6_M1lSw1NA4yTZS8HHkl/view?usp=sharing).

## Step 3 : Play music
Now that you have configured the module and tested it, you can start to code your MP3 player. With the Arduino IDE, make somes function to play music, change the music, stop the music and change the volume.

[Here an exemple](https://create.arduino.cc/example/builtin/02.Digital%5CButton/Button/preview) of how to use a button with the Arduino IDE.

[Here a tutorial](https://lastminuteengineers.com/rotary-encoder-arduino-tutorial/) of how to use a rotary encoder with exemple with the Arduino IDE.

## How to code with arduino
When you create a new project with arduino, you have to create a function called **setup()** and a function called **loop()**. The **setup()** function is called only one time when the arduino is powered on. The **loop()** function is called in a loop. You can use the **setup()** function to initialize your variables and the **loop()** function to read the inputs and do the actions.

You can also use #define to define your pins. For example, if you want to define the pin 2 as the pin of your button, you can write :
```c
#define BUTTON_PIN 2
```

Example in image : ![arduino](https://i.imgur.com/YwIaJ6v.png)


