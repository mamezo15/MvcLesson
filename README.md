# 研修で学んだVB.Net MVCの基礎

VisualBasicでMVC開発に携わることになりプログラミングの研修がありました。
その研修で出ました課題をここに残したいと思います。

僕自身の勉強のためにも完成したものはここに挙げたいと思います。
※Lessonのラスト問題を解いたもののみになります。

## Lesson1
### Lesson1-1

For文を使い1~100まで表示する

### Lesson1-2

3の倍数は()で囲む

### Lesson1-3

8の倍数は{}で囲む

### Lesson1-4
10の倍数は[]で囲む

### Lesson1-5
数字を渡すと上記の処理を行う関数を作成する。

### Lesson1-6
配列を作成して平均を求める
Dim arrayScore() As Integer = {50, 40, 80, 40, 0}

### Lesson1-7
配列を受け平均を返す関数の作成

#### 完成したもの
パスを書くか

## Lesson2
### Lesson2-1
ログイン画面を作る
ログインできるユーザは「UserID:saitou PassWord:makoto」のみ
ログインできた場合はログイン成功画面を表示する。
ログイン認証はモデルで行い、空判定はコントローラーで行う。

ログイン情報を入力してください。
UserID:  【    】※空の場合はエラーメッセージを表示
PassWord:【    】※空の場合はエラーメッセージを表示
【ログイン】
※ログイン情報が間違っていた場合はエラーメッセージを表示


### Lesson2-2
ログインできるユーザを追加する。
「UserID:ishibashi PassWord:makoto」

### Lesson2-3
ログイン後のページをユーザごとに変える。
なおビューはひとつでURLはQueryStringを利用し saitouユーザは「/Login/MainMenu?MODE=1」、ishibashiユーザは「/Login/MainMenu?MODE=2」とする
ビューの表示についてはRazer構文を利用してユーザごとに表示を変える。

### Lessoon2-4
ここまで作成したログインページには問題があります。
saitouでログインしたあとURLを~/Login/MainMenu?MODE=1　から ~/Login/MainMenu?MODE=2に変更すると
ishibashiでログインしたことになってしまう。(逆も同様)
Cookieを利用し上記のような操作に対して制御を行い、不正にアクセスした場合には「不正アクセスはやめてください」と表示する

#### 完成したもの
