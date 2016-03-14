# The Number of Island

地勢を示す縦 12, 横 12 のマスからなる平面図があります。おのおののマスは白か黒に塗られています。白は海を、黒は陸地を表します。二つの黒いマスが上下、あるいは左右に接しているとき、これらは地続きであるといいます。この平面図では、黒いマス一つのみ、あるいは地続きの黒いマスが作る領域を「島」といいます。例えば下図には、5 つの島があります。

    ■■■■□□□□■■■■
    ■■■□□□□□■■■■
    ■■□□□□□□■■■■
    ■□□□□□□□■■■■
    □□□■□□□■□□□□
    □□□□□□■■■□□□
    □□□□□■■■■■□□
    ■□□□■■■■■■■□
    ■■□□□■■■■■□□
    ■■■□□□■■■□□□
    ■■■■□□□■□□□□
    □□□□□□□□□□□□

マスのデータを読み込んで、それぞれの島の数を出力して終了するプログラムを作成してください。

## Input

黒いマスを 1、白いマスを 0 で表現した 12 個の数字の列 12 行でひとつの平面図を表します。 平面図と平面図の間は空白行で区切ります。入力例を参考にして下さい。

## Constraints

平面図の数は20を超えません。

## Output

島の数（1 件目のデータに対する出力）  
島の数（2 件目のデータに対する出力）  
...  
...  

## Sample Input

    111100001111
    111000001111
    110000001111
    100000001111
    000100010000
    000000111000
    000001111100
    100011111110
    110001111100
    111000111000
    111100010000
    000000000000

    010001111100
    110010000010
    010010000001
    010000000001
    010000000110
    010000111000
    010000000100
    010000000010
    010000000001
    010010000001
    010010000010
    111001111100

    000000000000
    111111111111
    100010100001
    100010100001
    100010100001
    100010100001
    100100100101
    101000011101
    100000000001
    100000000001
    111111111111
    100000000001

## Output for the Sample Input

    5
    13
    4

## Hint

以下はサンプルインプットを■と□で表したものです。

    ■■■■□□□□■■■■　　□■□□□■■■■■□□　　□□□□□□□□□□□□
    ■■■□□□□□■■■■　　■■□□■□□□□□■□　　■■■■■■■■■■■■
    ■■□□□□□□■■■■　　□■□□■□□□□□□■　　■□□□■□■□□□□■
    ■□□□□□□□■■■■　　□■□□□□□□□□□■　　■□□□■□■□□□□■
    □□□■□□□■□□□□　　□■□□□□□□□■■□　　■□□□■□■□□□□■
    □□□□□□■■■□□□　　□■□□□□■■■□□□　　■□□□■□■□□□□■
    □□□□□■■■■■□□　　□■□□□□□□□■□□　　■□□■□□■□□■□■
    ■□□□■■■■■■■□　　□■□□□□□□□□■□　　■□■□□□□■■■□■
    ■■□□□■■■■■□□　　□■□□□□□□□□□■　　■□□□□□□□□□□■
    ■■■□□□■■■□□□　　□■□□■□□□□□□■　　■□□□□□□□□□□■
    ■■■■□□□■□□□□　　□■□□■□□□□□■□　　■■■■■■■■■■■■
    □□□□□□□□□□□□　　■■■□□■■■■■□□　　■□□□□□□□□□□■

* * *

Source: PC Koshien 2004 , All-Japan High School Programming Contest, Aizu-Wakamatsu, Japan, 2004   
<http://www.pref.fukushima.jp/pc-concours/>