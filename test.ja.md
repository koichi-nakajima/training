---
title: "Check markdown with escape (backslash)"
weight: 9999
---

マークダウン翻訳の実験です。

{{%service%}}の画面を、HTMLの\<frame>または\<iframe>タグを使用してほかの<span class="notranslate">Webサイト</span>や普段よく使っているシステムなどの画面に埋め込む場合に必要な設定について説明します。初期設定では、{{%service%}}共通管理画面でクリックジャッキングからの保護が有効になっています。\<frame>または\<iframe>タグを使用した埋め込みを行う場合は、クリックジャッキングからの保護を無効にします。
{{% note %}}この％ｎｏｔｅ％は1行の中にタグ部分も書いています。![保存ボタン](/k/img-ja/save.png) をクリックします。{{% /note %}}
{{% note %}}

*   ファイルの形式によって、次の制限事項があります。  
    **Excelブック形式でファイルを作成する場合**
    
    *   1,000件までのレコードを登録できます。
    *   読み込めるファイルの最大サイズは1MB、拡張子は「.xlsx」です。
    
    **CSV形式でファイルを作成する場合**

    *   10万件までのレコードを登録できます。
    *   読み込めるファイルの最大サイズは100MBです。

{{% /note %}}

{{% note %}}
{{% subtitle %}}タイトル{{% /subtitle %}}
これは補足です。これは補足です。これは補足です。これは補足です。これは補足です。
{{% /note %}}


こっちは％マークを使って、空白行無しでマークダウンを記述してみる。
{{% note %}}
*   ファイルの形式によって、次の制限事項があります。  
    **Excelブック形式でファイルを作成する場合**
    
    *   1,000件までのレコードを登録できます。
    *   読み込めるファイルの最大サイズは1MB、拡張子は「.xlsx」です。
    
    **CSV形式でファイルを作成する場合**

    *   10万件までのレコードを登録できます。
    *   読み込めるファイルの最大サイズは100MBです。
{{% /note %}}
次のいずれかの種類のフィールドをキーにできます。

* レコード番号\*<br>
* 文字列（1行）\*\*<br>
* 数値\*\*<br>
* 日付\*\*<br>
* 日時\*\*<br>
* リンク\*\*

\* レコード番号をキーにする場合、キーに指定したファイルの列にアプリに存在しないレコード番号があると、ファイルを読み込めません。<br>
\*\* フィールドの「値の重複を禁止する」設定を有効にしている必要があります。

1. アプリのレコードの一覧画面を開きます。
1. ![漏斗アイコン](/k/img/filter.png)をクリックしてThis is a test note、レコードの一覧に表示されるレコードを絞り込みます。
{{% note %}}

ここで指定した条件にあてはまるレコードだけがファイルに書き出されます。
{{% /note %}}
{{< screen src="/k/img-ja/data_export_img02.png"  alt="画像">}}
{{% warning %}}

* アクションの利用者には、次の権限が必要です。
 * コピー元のフィールドの閲覧権限
 * コピー先のアプリへのレコードの追加権限
 * コピー先のフィールドの編集権限
{{% /warning %}}
{{< seealso title="関連する記事" >}}
[アクセス権の設定](/k/ja/user/app_settings/rights.html)
{{< /seealso >}}

<br>
ここから下は、HTMLでTableが書かれている。

<table>
<caption>サムネイルの表示の設定による表示の違い</caption>
    <thead>
        <tr>
            <th>サムネイルの表示の設定</th>
            <th>表示例</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="width: 234.3px;">有効</td>
            <td style="width: 234.7px;">サムネイルが表示されます。
            <br>
            例：
            <br>
            {{< screen src="/k/img-ja/thumbnail_img1_1.png"  alt="画像">}}
            </td>
        </tr>
        <tr>
            <td>無効</td>
            <td>ファイル名が表示されます。<br>
            例：
            <br>
            {{< screen src="/k/img-ja/thumbnail_img2_1.png"  alt="画像">}}
            </td>
        </tr>
    </tbody>
</table>

{{% note %}}

画像のファイルサイズが10MBを超える場合、サムネイルの設定に関わらず、ファイル名が表示されます。サムネイルは表示されません。
{{% /note %}}

## ここから下は、escape、つまりバックスラッシュ(\)付きで行頭の文字を書いています。

\\   backslash

\`   backtick

\*   asterisk

\_   underscore

\{\}  curly braces

\[\]  square brackets

\(\)  parentheses

\#   hash mark

\+   plus sign

\-   minus sign (hyphen)

\.   dot

\!   exclamation mark

## ここから下は、escape、つまりバックスラッシュ(\)無しで行頭の文字を書いています。

\   backslash

`   backtick

*   asterisk

_   underscore

{}  curly braces

[]  square brackets

()  parentheses

#   hash mark

+   plus sign

-   minus sign (hyphen)

.   dot

!   exclamation mark

## ここから下は、行頭ではなく普通の文章内に記号を書いてみます。

最初はescape付き、次はescape無しです。

こんな感じ＼こんな感じ＼＼こんな感じ

バックスラッシュ\バックスラッシュ\\バックスラッシュ

バッククォート`バッククォート（backtick）\`バッククォート

アステリスク*アステリスク\*アステリスク

下線_下線\_下線

波かっこペア{}波かっこペア\{\}波かっこペア

波かっこ開き{波かっこ開き\{波かっこ開き

波かっこ閉じ}波かっこ閉じ\}波かっこ閉じ

角かっこペア[]角かっこペア\[\]角かっこペア

角かっこ開き[角かっこ開き\[角かっこ開き

角かっこ閉じ]角かっこ閉じ\]角かっこ閉じ

丸かっこペア()丸かっこペア\(\)丸かっこペア

丸かっこ開き(丸かっこ開き\(丸かっこ開き

丸かっこ閉じ)丸かっこ閉じ\)丸かっこ閉じ

ハッシュ#ハッシュ\#ハッシュ

プラス+プラス\+プラス

マイナス-マイナス\-マイナス

ドット.ドット\.ドット

ビックリ!ビックリ\!ビックリ

### ここから下は、サンプルです。

* レコード番号\*<br>
* 文字列（1行）\*\*<br>
* 数値\*\*<br>
* 日付\*\*<br>
* 日時\*\*<br>
* リンク\*\*

この下の2行は、アステリスク(*)をescapeしてます。

\* レコード番号をキーにする場合、キーに指定したファイルの列にアプリに存在しないレコード番号があると、ファイルを読み込めません。<br>
\*\* フィールドの「値の重複を禁止する」設定を有効にしている必要があります。

* レコード番号*<br>
* 文字列（1行）**<br>
* 数値**<br>
* 日付**<br>
* 日時**<br>
* リンク**

この下の2行は、最初の行はescape付き、2行目は単に"**"を書いています。

\* レコード番号をキーにする場合、キーに指定したファイルの列にアプリに存在しないレコード番号があると、ファイルを読み込めません。<br>
** フィールドの「値の重複を禁止する」設定を有効にしている必要があります。
