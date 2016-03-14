# Taro's Obsession

まんじゅう好きの太郎くんの家でたいへんな事件がおきました。和室の仏壇に供えてあった3つのまんじゅうのうち1つが無くなっていたのです。いつかはおやつにいただこうと狙っていた太郎くんが犯人を見つけるため捜査を始めると、その日、和室に入った人が何人もいることが分かりました。そこで、これらの容疑者が部屋に入った順序を調べるため、全員に次のような形式の証言をしてもらうことにました。

容疑者 A の証言 「私は容疑者 B より先に部屋に入った。」

容疑者の一人(?)は三毛猫のタマなので証言はできませんが、幸運にも最後に部屋に入ったところを太郎くんは見ていました。

太郎くんはこれらの証言から、部屋に入った順番を推測して捜査に役立てることにしました。

例えば、6 人の容疑者がいてタマを容疑者 2 とした場合、以下のような証言が得られたとします。

容疑者 5 の証言 「私は 2 より先に部屋に入った。」  
容疑者 1 の証言 「私は 4 より先に部屋に入った。」  
容疑者 3 の証言 「私は 5 より先に部屋に入った。」  
容疑者 4 の証言 「私は 2 より先に部屋に入った。」  
容疑者 1 の証言 「私は 6 より先に部屋に入った。」  
容疑者 6 の証言 「私は 4 より先に部屋に入った。」  
容疑者 3 の証言 「私は 4 より先に部屋に入った。」  

この証言をつなぎ合わせると、部屋に入った順序は

* 3→5→1→6→4→2
* 1→6→3→4→5→2
* 3→1→6→5→4→2

など、何通りかの可能性に絞り込むことができます。

というわけで、タマ(容疑者 2 )以外の容疑者全員の証言から、部屋に入った順番を推測し、可能性のある順番の 1 つを出力して終了するプログラムを作成してください。ただし、容疑者の人数を m とすると m は 20 以下であり、容疑者は 1 から m までの整数で識別されます。証言の数は 100 以下とします。また、複数の証言をする容疑者がいるかもしれませんが、どの証言も真実であり矛盾していないものとします。

## Input

1 行目は、容疑者の人数 m(整数)  
2 行目は、証言の数 n(整数)  
3 行目からは、証言の内容 x y(整数空白区切り)  
x y:容疑者 x(私)は容疑者 y より先に入った。  
:  
:  
n 2 行目は、n 番目の証言  

## Output

最初に部屋に入った容疑者の番号(整数)  
2 番目に部屋に入った容疑者の番号(整数)  
:  
:  
m 番目に部屋に入った容疑者の番号(整数)  

## Sample Input

    6
    7
    5 2
    1 4
    3 5
    4 2
    1 6
    6 4
    3 4

## Output for the Sample Input

    3
    5
    1
    6
    4
    2

* * *

Source: PC Koshien 2005 , All-Japan High School Programming Contest, Aizu-Wakamatsu, Japan, 2005   
<http://www.pref.fukushima.jp/pc-concours/>