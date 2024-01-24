# Building Guide

- [中文說明（Chinese Guide）](guide.md)。
- 英文說明（English Guide）。

## Pre-operation

- After printing out all the parts needed for the keyboard, first take out the bottom parts and spacers ,follow the photo instructions for installing the posts in their proper locations.

![](pics/g03.jpg)

- Next, install the switches onto the plate and set them aside temporarily when you are done.

![](pics/g04.jpg)
![](pics/g05.jpg)
![](pics/g06.jpg)

## Diodes and Single PCB

- Here is a brief explanation of the orientation of the diode on the single PCB, please follow the photo below to install the diode on the PCBs.

![](pics/g08.png)
![](pics/g09.jpg)

- Next step you need to solder the diodes, then cut off the useless feets.

![](pics/g10.jpg)
![](pics/g11.jpg)

- The completed single PCBs are then mounted onto the positioning plate and soldered in place.

![](pics/g12.jpg)
![](pics/g13.jpg)

- It has a switche on the PCB for EC-11, don't forget to install the diode on it.

![](pics/g21.jpg)
![](pics/g22.jpg)

- After installing the diode, you can fix the knob on the board first.

![](pics/g23.jpg)

## Link Keyboard Matrix

- The following photo shows the matrix of the MagWave44. Since all the plates are divided into 6 pieces, first we need to connect the single PCBs in the photo with wires.

![](pics/g16.png)

- That's how it feels when it's done.

![](pics/g14.jpg)

## PCBs

> **Note**
>
> The part of the main board contains MCU, Body, EC-11 and TRRS, please prepare them first.

![](pics/g17.jpg)

- The MCU board part is not divided into front and back, you can adjust the direction, this time it is to install a split keyboard, the part of the bus connector is facing the left and right side respectively.

![](pics/g24.jpg)

- Next, solder the MCU (here I used RP2040-matrix to be MCU) on the MCU board in the desired way.

![](pics/g25.jpg)

- The TRRS jacks are then soldered to the dedicated PCB board.

![](pics/g26.jpg)

> **Note**
>
> The left and right sides of the MCU have several usable IOPins, so solder as many female pins as you want to the bus connector labeled.

> **Note**
>
> The following photo shows the main functions of the board, MagWave44 will use Power, TRRS (VCC, S1, GND), Signal (S1, A1, B1), Rotray Encoder (A1, GND, B1), and Matrix (Row and Col), and will be left and right side of the board the corresponding row of pins female sockets soldering fixed.

![](pics/g20.png)
![](pics/g27.jpg)
![](pics/g28.jpg)

- 然後將它們分別用M2x8mm螺絲、M2螺帽固定在底板上。（這裡我有搭配墊片，可視需求使用）

![](pics/g29.jpg)

## 接線原理

> **Note**
>
> 如果是想依照MagWave44相應的韌體進行接線的話，下圖會說明各類MCU要如何接線比較輕鬆容易：

1. ATMega32U4 ProMicro, Elite-C:
![](pics/elitec.png)

2. RP2040 ProMicro系列:
![](pics/RP2040ProMicro.jpg)

3. RP2040-Zero, RP2040Supermini, RP2040-Matrix (板載RPG矩陣):
![](pics/RP2040SueprMini0.png)









