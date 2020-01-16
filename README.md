# vi_memo_to_self

### vi (vim) 備忘録

自分用メモ

---

### 終了 / 保存

```
:q!
# 強制終了(Escを事前連打)

:q
# そのまま終了

:wq
# 上書き保存＋終了

:w
# 上書き保存
```

---

### 移動（コマンドモード）

```
0 (or ^)
# 行アタマへ移動

$
# 行の末へ移動
```
```
b
# 前の単語へ移動

w
# 次の単語へ移動（word）

e
# 現単語の最後文字に移動
```
```
gg
# 最初の行へ移動

G
# 最終の行へ移動

:number_hoge
# 指定した行ナンバー場所へ移動  (e.g. ":5" など)
```
```
ctl + b
# 前ページへ移動

ctl + f
# 次ページへ移動
```
```
h　j　k　l
# 左・下・上・右 にそれぞれ移動
```

---

### 取り消し／やり直し（コマンドモード）

```
u
# 取り消し

Ctr + r
# やり直し
```

---

### 文字列編集（コマンドモード）

```
x
# カーソル位置の文字カット

dd
# 行をカット

yy
# 行ヤンク

p
# プット

/word_wanted
# 文字列検索
```

---

### 文字列編集（コマンドモードからINSEARTモードに切り替わる。変換用に！）

```
cw
# 一文字変換

dw
# 一単語を削除
```

---

### 行ナンバー表示（コマンドモード）

```
:set nu
# オン

:set nonu
# オフ
```

---

### その他メモ

#### vi (ヴイアイ)

- Windowsでいうメモ帳の __Linux版__ (みたいなもの)


    ```
    # vi / vim での入り方

    $ vi hoge.txt

    $ vim hoge.txt
    ```

#### コマンドモード / 文字入力モード

おもに2つのモードがある。

- コマンドモード

  - 終了・保存・行削除 など

- 文字入力モード

  文字挿入・書き込み

  1. 起動  (直後はコマンドモードになってる)
  1. __文字入力モード__ へ切り替え
  1. __コマンドモード__ へ切り替え
  1. 終了


