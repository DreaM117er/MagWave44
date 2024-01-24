# 組裝說明

- 中文說明（Chinese Guide）。
- [英文說明（English Guide）](guide_en.md)。

## 前置作業

- 列印完所有鍵盤需要的部件後，首先將底板及銅柱拿出來，並依照照片指示將銅柱安裝到適當的位置上。

![](pics/g03.jpg)

- 接著將鍵軸安裝到定位板上，完成後再將它們暫時放一邊。

![](pics/g04.jpg)
![](pics/g05.jpg)
![](pics/g06.jpg)

## 二極體及單格電路板

- 這裡簡單說明單格電路板上的二極體方向，請按照下圖將二極體安裝到單格電路板上。

![](pics/g08.png)
![](pics/g09.jpg)

- 接著將二極體用焊錫固定好，再剪去多餘的腳。

![](pics/g10.jpg)
![](pics/g11.jpg)

- 再來將已經完工的單格電路板安裝到定位板上焊接固定。

![](pics/g12.jpg)
![](pics/g13.jpg)

- EC-11電路板上還有一個按鈕，不要忘記將二極體接上去。

![](pics/g21.jpg)
![](pics/g22.jpg)

- 接好二極體後，可以先將旋鈕固定在板子上備著。

![](pics/g23.jpg)

## 連結矩陣

- 下圖是MagWave44的矩陣圖，由於定位板合計分成6塊，首先我們需要將圖中的單格電路板用電線接起來。

![](pics/g16.png)

- 完成後會是這樣的感覺。

![](pics/g14.jpg)

## 電路板

> **Note**
>
> 主體電路板的部分包含`MCU`、`本體`、`TRRS`、`EC-11`，請先將他們備著。

![](pics/g17.jpg)

- MCU電路板的部分因為它沒有分正反面，你可以任意調整方向，這次是安裝分離式鍵盤，匯流排線接口的部分分別朝向左右邊。

![](pics/g24.jpg)

- 接著將MCU（這裡我是使用`RP2040-Matrix`做為主控）按照理想的方式固定在MCU電路板上。

![](pics/g25.jpg)

- 接著再將`TRRS座`也焊接固定在專用的PCB板上。

![](pics/g26.jpg)

> **Note**
>
> MCU左右邊有幾個可使用的IOPin，就焊接多少母排針座到匯流排線座的標示上。

> **Note**
>
> 下圖是本體電路板的主要功能說明，MagWave44會用到`Power`、`TRRS`（`VCC`、`S1`、`GND`）、`Signal`（`S1`、`A1`、`B1`）、`Rotray Encoder`（`A1`、`GND`、`B1`）及`Matrix`（`Row`及`Col`）的部分，並將左右邊本體電路板相應的排針母座焊接固定好。

![](pics/g20.png)
![](pics/g27.jpg)
![](pics/g28.jpg)

- 然後將它們分別用`M2x8mm螺絲`、`M2螺帽`固定在底板上。（這裡我有搭配`墊片`，可視需求使用）

![](pics/g29.jpg)

## 接線原理

> **Note**
>
> 如果是想依照MagWave44`相應的韌體`進行接線的話，下圖會說明各類MCU要如何接線比較輕鬆容易：

|微控制器|示意圖|
|---|---|
|`ATMega32U4 ProMicro`、`Elite-C`|![](pics/elitec.png)|
|`RP2040 ProMicro`系列|![](pics/RP2040ProMicro.jpg)|
|`RP2040-Zero`、`RP2040Supermini`、`RP2040-Matrix `|![](pics/RP2040SueprMini0.png)|

> **Warning**
>
> `ProMicro`、`Elite-C`有著相同的IOPin；`RP2040-Zero`、`RP2040Supermini`、`RP2040-Matrix `三者也一樣。

> **Note**
>
> 接著按照順序將MCU上的線路接到本體板上，再將本體向外接線接出去。
> 
> 請依照自己的手拉線技巧將線路一步步接起來，我的方式是將電線組合成排線，再將它們接到相應的位置上。

- 連結TRRS座:

![](pics/g31.jpg)
![](pics/g32.jpg)
![](pics/g33.jpg)
![](pics/g33.jpg)
![](pics/g35.jpg)
![](pics/g34.jpg)
![](pics/g30.jpg)

- 給鍵盤本體供電:

![](pics/g36.jpg)
![](pics/g37.jpg)
![](pics/g38.jpg)

- 連結MCU到Signal，還有旋鈕EC-11: （我忘了拍照...）

![](pics/g39.jpg)
![](pics/g40.jpg)
![](pics/g41.jpg)
![](pics/g42.jpg)
![](pics/g43.jpg)

- EC-11旋鈕的矩陣圖:

![](pics/c3.png)
![](pics/g44.jpg)

- 小指區域的矩陣圖:

![](pics/c1.png)
![](pics/g45.jpg)
![](pics/g46.jpg)

- 拇指區域的矩陣位置:

![](pics/c4.png)
![](pics/g47.jpg)
![](pics/g48.jpg)

- 最後將主要按鍵區域裝上去:

![](pics/c2.png)
![](pics/g49.jpg)
![](pics/g50.jpg)

- 然後完成另一支手：

![](pics/g51.jpg)

- 接著測試鍵盤按鍵、矩陣及旋鈕有沒有正常運作。

![](pics/g52.jpg)

- 最後把鍵帽安裝上去就完成了。

![](pics/g53.jpg)

## 鍵盤腳撐

> **Note**
>
> MagWave44有2種方式自行添加不同角度的腳撐，一種是是M5螺絲安裝在鍵盤周圍的4個角落，一種是使用Magsafe引磁片，需要搭配Magsafe雲台座合併使用。

- Magsafe引磁片：

![](pics/o01.jpg)
![](pics/o02.jpg)
![](pics/o03.jpg)

- M5螺絲腳撐

![](pics/o04.jpg)
![](pics/o05.jpg)

- Magsafe雲台座，搭配雲台配件使用：

![](pics/o06.jpg)
![](pics/o07.jpg)
![](pics/o08.jpg)