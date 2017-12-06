# Wiegand Reader for Raspberry Pi

![Fritzing](<img align="left" width="583" height="437" src="/images/image1.png">) ![Cable attachments](<img align="right" width="642" height="297" src="/images/image2.png">)

| Wires | Function |
| ------ | ------ |
| Red | Typical operation 5V-12V -- 3.3V + 5V from GPIO is connected |
| Black | Ground |
| Green | Data 0 - Logic 5V coming out, regulate down to 3.3V for rPi GPIO|
| White | Data 1 - Logic 5V coming out, regulate down to 3.3V for rPi GPIO|
| Yellow | Programmatic Beep Control (Reader beeps when Yellow is set to ground) |

To compile:
```sh
$ gcc -lpthread -lwiringPi -lrt hello.c -o hello
```
