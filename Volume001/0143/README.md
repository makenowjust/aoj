# Altair and Vega

織女は天帝の子供でしたが、父の言いつけであけてもくれても機を織っていました。

織女のおる雲錦という見事な布で仕立てた服を着るのが天帝の楽しみでした。雲錦は寿命が短くすぐ に劣化してしまいますが、働き者の織女が毎日織ってくれるので、問題はありませんでした。織女は、 父の言いつけを守り、毎日毎日雲錦を織り続けていたので、ボーイフレンドはいませんでした。かわい そうに思った父は、天の川の向こう岸に住む牽牛という働き者を紹介してやり、嫁入りさせました。

すると、織女は、結婚の楽しさに夢中になって、機織りなどそっちのけで、牽牛と遊び呆けていま す。天帝のお気に入りの雲錦の服も新しく仕立てられないためボロボロになってしまいました。

これには、父も怒って織女を宮殿に連れ戻したいと思いました。しかし人間である牽牛の前にボロボ ロの服で姿を現すわけにはいきません。遊び呆けている二人を3角形の壁で遮断し自分以外の全てのも のが行き来できなくすることを考えました。そして、牽牛に見つからずに、織女に会って、まじめに機 を織るか、さもなければ強制的に連れ帰ると宣言するというのです。

![][1]

天帝はこの作戦遂行のために3角形の壁生成装置の開発を開発部署に命じました。3点を与えてそこに壁 を作るという仕様で発注したつもりでしたが、開発部署では何を間違えたのか、ランダムに(無作為 に)に3角形の壁を生成し、その3点を報告するシステムを作ってしまいました。発注者として、天帝は 作り直しを命じたいのですが、服がますますボロボロになったので、最小限の手直しで手を打つことに しました。ランダムに壁ができたのではたまったもんじゃないので、作ろうとする3角形が決まった段 階で、3点を報告し、それで満足するものならば(すなわち遮断ができていれば)天帝がOKボタンを押 して壁の作成を指示するという仕様にしました。遮断できていなければ(遮断不全ならば)NGボタンを 押し、やり直しとなります。織女と牽牛は時々刻々場所を変えます。壁生成装置からは無作為の3点が どんどん出力されてきます。

天帝は与えられた状況下で、壁の作成を指示すべきか否かを判定する必要に迫られました。そこで、 天帝にかわり、3角形の3頂点の位置(xp1,yp1),(xp2,yp2),(xp3,yp3)、牽牛の位置(xk,yk)、および織女 の位置(xs,ys)、を入力とし、三角形が牽牛と織女を遮断しているか否かを判定し、遮断できている場 合はOK、遮断できていない場合にはNGを出力し終了するプログラムを作成してください。ただし、遮断 しているとは、牽牛と織女のいずれかが三角形の内側にあり、他方が外側にある場合を言います。牽牛 と織女は三角形の頂点もしくは辺の上にはいないものとします。

## Input

    1行目 判別したい情報の個数n(整数)
    2行目 第1の位置情報 xp1 yp1 xp2 yp2 xp3 yp3 xk yk xs ys(整数;半角空白区切り)
           三角形の3頂点の位置(xp1,yp1),(xp2,yp2),(xp3,yp3)
           牽牛の位置(xk,yk)
           織女の位置(xs,ys)
    3行目 第2の位置情報 xp1 yp1 xp2 yp2 xp3 yp3 xk yk xs ys(整数;半角空白区切り)
           :
           :
    n 1行目 第nの位置情報 xp1 yp1 xp2 yp2 xp3 yp3 xk yk xs ys(整数;半角空白区切り)

## Output

    1行目 第1の位置情報の判定結果OKまたはNG(半角英字)
    2行目 第2の位置情報の判定結果OKまたはNG(半角英字)
        :
        :
    n行目 第nの位置情報の判定結果OKまたはNG(半角英字)

## Sample Input

    5
    2 5 9 2 8 9 2 11 6 5
    2 5 9 2 8 9 2 11 12 6
    2 5 9 2 8 9 2 11 11 9
    14 1 25 7 17 12 17 9 20 5
    14 1 25 7 17 12 22 13 20 5

## Output for the Sample Input

    OK
    NG
    NG
    NG
    OK

* * *

Source: PC Koshien 2006 , All-Japan High School Programming Contest, Aizu-Wakamatsu, Japan, 2006   
<http://www.pref.fukushima.jp/pc-concours/>

[1]: IMAGE1/altairAndVega.gif