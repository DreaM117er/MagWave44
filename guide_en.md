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

- After installing the diode, you can solder EC-11 on the board first.

![](pics/g23.jpg)

## Link Keyboard Matrix

- The following photo shows the matrix of the MagWave44. Since all the plates are divided into 6 pieces, first we need to connect the single PCBs in the photo with wires.

![](pics/g16.png)

- That's how it feels when it's done.

![](pics/g14.jpg)

## PCBs

> **Note**
>
> The part of the main board contains `MCU`, `Body`, `EC-11` and `TRRS`, please prepare them first.

![](pics/g17.jpg)

- The MCU board part is not divided into front and back, you can adjust the direction, this time it is to build a split keyboard, the part of the bus connector is facing the left and right side respectively.

![](pics/g24.jpg)

- Next, solder the MCU (here I used `RP2040-matrix` to be MCU) on the MCU board in the desired way.

![](pics/g25.jpg)

> **Note**
>
> After solder the MCU on the MCU board, the `left side pin` will lead to the `L side`, the `right side` will lead to the `R side`, and the `bottom side` will lead to the `D side` below, and the direction of the `arrow` will be the position of the pin as the direction reading.

- The `TRRS jacks` are then soldered to the dedicated PCB board.

![](pics/g26.jpg)

> **Note**
>
> The left and right sides of the MCU have several usable IOPins, so solder as many female pins as you want to the bus connector labeled.

> **Note**
>
> The following photo shows the main functions of the board, MagWave44 will use `Power`, `TRRS` (`VCC`, `S1`, `GND`), `Signal` (`S1`, `A1`, `B1`), `Rotray Encoder` (`A1`, `GND`, `B1`), and `Matrix` (`Row` and `Col`), and will be left and right side of the board the corresponding row of pins female sockets soldering fixed.

![](pics/g20.png)
![](pics/g27.jpg)
![](pics/g28.jpg)

- Then fasten them to the bottom case with `M2x8mm screws` and `M2 nuts` respectively. (Here I have the matching `washers`, you can use it according to your needs)

![](pics/g29.jpg)

## Wiring Principle

> **Note**
>
> If you want to wire the MCUs according to the MagWave44 `firmwares`, the following photo shows how to wire the MCUs in an easy way:

|MCUs|Photo|
|---|---|
|`ATMega32U4 ProMicro`, `Elite-C`|![](pics/elitec.png)|
|`RP2040 ProMicro` series|![](pics/RP2040ProMicro.jpg)|
|`RP2040-Zero`, `RP2040Supermini`, `RP2040-Matrix`|![](pics/RP2040SueprMini0.png)|

> **Warning**
>
> `Elite-C`, `ProMicro` have same count of IOPins; `RP2040-Zero`, `RP2040Supermini`, `RP2040-Matrix` also too.

> **Note**
>
> Next, connect the wires from the MCU to the body board in order, and then connect the body to the external wires.
> 
> Please follow your own handwiring skills to connect the wires step by step, the way I do it is to assemble the wires combine arrays and then connect them to the corresponding sites.

- Connect TRRS jack:

![](pics/g31.jpg)
![](pics/g32.jpg)
![](pics/g33.jpg)
![](pics/g33.jpg)
![](pics/g35.jpg)
![](pics/g34.jpg)
![](pics/g30.jpg)

- Give Power onto the body board:

![](pics/g36.jpg)
![](pics/g37.jpg)
![](pics/g38.jpg)

- MCU to Signal, and connect EC-11: (I forgot to take Signal photo...)

![](pics/g39.jpg)
![](pics/g40.jpg)
![](pics/g41.jpg)
![](pics/g42.jpg)
![](pics/g43.jpg)

- Matrix of EC-11:

![](pics/c3.png)
![](pics/g44.jpg)

- Matrix of Col0-1, Row0-3 (little finger area):

![](pics/c1.png)
![](pics/g45.jpg)
![](pics/g46.jpg)

- Matrix of Col3-5, Row3 (Thumb area):

![](pics/c4.png)
![](pics/g47.jpg)
![](pics/g48.jpg)

- Matrix of Col2-5, Row0-3 (Main area):

![](pics/c2.png)
![](pics/g49.jpg)
![](pics/g50.jpg)

- Then finish other hand side:

![](pics/g51.jpg)

- Testing keyboard, matrix and RGB led work.

![](pics/g52.jpg)

- Put on your keycaps, then all done.

![](pics/g53.jpg)

## Tending

> **Note**
>
> The MagWave44 has two ways to add the tending at different angles, one is by using the M5 screws in the 4 corners around the keyboard, and the other is by using the Magsafe rings, which need to be combined with the Magsafe tripod.

- Magsafe rings:

![](pics/o01.jpg)
![](pics/o02.jpg)
![](pics/o03.jpg)

- M5 screws tending:

![](pics/o04.jpg)
![](pics/o05.jpg)

- Magsafe tripod and crema tripod.

![](pics/o06.jpg)
![](pics/o07.jpg)
![](pics/o08.jpg)