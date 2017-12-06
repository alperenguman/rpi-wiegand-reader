# Wiegand Reader for Raspberry Pi

Use this repository to read RFID cards with the Raspberry Pi.

| Wires | Function |
| ------ | ------ |
| Red | Typical operation 5V-12V -- 3.3V + 5V from GPIO is connected |
| Black | Ground |
| Green | Data 0 - Logic 5V coming out, regulate down to 3.3V for rPi GPIO|
| White | Data 1 - Logic 5V coming out, regulate down to 3.3V for rPi GPIO|
| Yellow | Programmatic Beep Control (Reader beeps when Yellow is set to ground) |

To compile:
```sh
$ gcc -lpthread -lwiringPi -lrt reader.c -o reader.o
```

##Sample output:
![Output](/images/image3.png)

##Wiring:
![Fritzing](/images/image2.png)
![Cable attachments](/images/image1.png)
