# vi_memo_to_self

### Vi / Vim チートシート

自分用メモ。

- Vimバージョン確認
    ```
    vim --version
    ```

---

### 移動（コマンドモード）

- 行アタマへ移動
    ```
    0 (or ^)
    ```

- 行の末へ移動
    ```
    $
    ```
- 前の単語へ移動
    ```
    b
    ```
- 次の単語へ移動（word）
    ```
    w
    ```
- 現単語の最後文字に移動
    ```
    e
    ```
- 最初の行へ移動
    ```
    gg
    ```
- 最終の行へ移動
    ```
    G
    ```
- 指定した行ナンバー場所へ移動  (e.g. ":5" など)
    ```
    :number_hoge
    ```
- 前ページへ移動
    ```
    ctl + b
    ```
- 次ページへ移動
    ```
    ctl + f
    ```
- 左・下・上・右 にそれぞれ移動
    ```
    h　j　k　l
    ```

---

### 取り消し／やり直し（コマンドモード）

- 取り消し
    ```
    u
    ```
- やり直し
    ```
    Ctr + r
    ```

---

### 文字列編集（コマンドモード）

- カーソル位置の文字カット
    ```
    x
    ```
- 行をカット
    ```
    dd
    ```
- 行ヤンク
    ```
    yy
    ```
- プット
    ```
    p
    ```
- 文字列検索
    ```
    /word_wanted
    ```

---

### 文字列編集（コマンドモードからINSEARTモードに切り替わる）

- 一文字変換
    ```
    cw
    ```
- 一単語を削除
    ```
    dw
    ```

---

### 終了 / 保存

- 強制終了(Escを事前連打)
    ```
    :q!
    ```
- そのまま終了
    ```
    :q
    ```
- 上書き保存＋終了
    ```
    :wq
    ```
- 上書き保存
    ```
    :w
    ```

---

## 設定（コマンドモード）

- 行ナンバー表示 オン/オフ
    ```
    :set nu

    :set nonu
    ```

- 言語のsyntaxを色付け オン/オフ
    ```
    :syntax on

    :syntax off
    ```

---

## その他メモ

#### Vi
- ヴイアイ
- Windowsでいうメモ帳の __Linux版__ (みたいなもの)

#### Vim
- ヴィム
- Viの機能拡張テキストエディタ
    > `$ vim --version` や `$ vim` 後の表示メッセージ:  
    > __VIM - Vi IMproved__
- 1980年代から開発が始まり、現在もさかんに改良が進められている。
    - [GitHubリポジトリ](https://github.com/vim/vim)

### Vi / Vim での入り方
- ファイル名を指定して実行（ファイルが存在しないときは新規ファイルが作成される）
    ```
    vi hoge.txt

    vim hoge.txt
    ```
- 別の方法：Vimを立ち上げてからファイルを開く
    ```
    vim
    ```
    ```
    :e file_name
    ```
    `:e` のあとにファイル名を指定して実行。

## コマンドモード / 文字入力モード

おもに2つのモードがある。

- コマンドモード（コマンドモード）
  - vimに入った直後のモード。
  - `:q`とか打てるモード。終了・保存・行削除 などカバー。
  - 移動や簡単な編集はなるべくコマンドラインモードで行うほうが強力。

- インサートモード（文字入力モード）

  文字挿入・書き込み

  1. 起動  (直後はコマンドモードになってる)
  1. __文字入力モード__ へ切り替え  __i__
  1. __コマンドモード__ へ切り替え  __Esc__
  1. 終了

#### その他モード
- ヴィジュアルモード

範囲指定

コピー

    - ヴィジュアルラインモード
    - ヴィジュアルブロックモード