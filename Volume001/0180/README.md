# Stellar Performance of the Debunkey Family

水の国ウォーターデブンにはn個の都市があります。各都市は水に囲まれており、島国のようになっています。ウォーターデブンには全部でm本の橋があり、都市間の交通はそれらの橋によって行われ、全ての都市に行き来することができます。最近、道路特定財源の見直しにより橋の維持費の削減が決定されました。全部の橋を維持することができなくなってしまい、いくつかの橋を取り壊すことになりました。そこで、ウォーターデブンはどの都市にでも行くことができるように橋を残しつつ、橋の維持費を最小化することが課題となりました。

都市の数、橋の数、各橋の維持費を入力とし、橋を利用してどの都市にも行けるようにしつつ、橋を取り壊した場合の維持費の最小値を出力するプログラムを作成してください。なお、橋の取り壊しはウォーターデブンの優秀な解体屋(デブンキー一家)により容易に行われ、取り壊しには費用が掛からないものとします。ただし、各都市は0からn-1まで順番に番号が付けられているものとし、さらに、都市の数は2以上100以下、橋の維持費は1以上100以下とします。

## Input

複数のデータセットの並びが入力として与えられます。入力の終わりはゼロふたつの行で示されます。各データセットは以下のとおりです。

    1行目   都市の数n 橋の数m(整数 整数;半角空白区切り)
    2行目   第1の橋の情報 a b cost(整数 整数 整数;半角空白区切り)
           各記号の意味は以下のようになります。
           a b:橋がつないでいる都市の番号
           cost:橋にかかる維持費
    3行目 第2の橋の情報
    4行目 第3の橋の情報
         :
    m 1行目 第mの橋の情報

## Output

入力データセット毎に橋の維持費の合計を出力します。

## Sample Input

    5 6
    0 2 1
    2 1 3
    2 3 8
    1 3 2
    3 4 5
    1 4 4
    3 3
    1 2 3
    2 0 3
    0 1 3
    0 0

## Output for the Sample Input

    10
    6

* * *

Source: PC Koshien 2008, Preliminary Round , All-Japan High School Programming Contest, Aizu-Wakamatsu, Japan, 2008   
<http://www.pref.fukushima.jp/pc-concours/>