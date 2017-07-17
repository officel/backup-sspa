# Learning Serverless Single Page Apps

## memo

* <a href="http://amzn.to/2tcqUc6">日本語版サーバレスシングルページアプリケーション本（オライリー）</a>の写経
* オリジナルは [benrady/learnjs: Prepared Workspace for "Serverless Single Page Apps" @ Pragprog](https://github.com/benrady/learnjs)

    * 若干中身が古いので少し変更
    * [normalize.css](https://github.com/necolas/normalize.css/) を 7.0.0 に
    * [jQuery](http://jquery.com/) を 3.2.1 に
    * [Skeleton](https://github.com/dhg/Skeleton/) は3年前で更新停止しているようだ
    * オリジナルの vendor.js の中の AWS SDK は導入の仕方が不明瞭なのとどうせすでに使い物にならないくらい古いはずなので使う段階になったら入れる

        * インストールされているはずなのは以下のとおり
        * CognitoIdentity
        * CognitoSync
        * DynamoDB
        * Lambda
        * STS

    * [jasmine](https://github.com/jasmine/jasmine) も [2.6.4](https://github.com/jasmine/jasmine/releases/tag/v2.6.4) に

          mkdir -p sspa/public/tests
          cd sspa/public/tests
          wget https://github.com/jasmine/jasmine/releases/download/v2.6.4/jasmine-standalone-2.6.4.zip
          unzip jasmine-standalone-2.6.4.zip
          mv SpecRunner.html index.html
          rm MIT.LICENSE
          rm -fr spec
          rm -fr src
          rm jasmine-standalone-2.6.4.zip
          cd lib/
          wget https://code.jquery.com/jquery-3.2.1.min.js
          cd ..
          vi index.html  // sspa/public/tests/index.html

    * オリジナルのリポジトリに書いてあるリンクに[原書のページ](https://pragprog.com/book/brapps/serverless-single-page-apps)
    * その中に[ソースコードのダウンロードへのリンク](https://pragprog.com/titles/brapps/source_code)
    * 日本語版書籍記載のソースコードは一部を抜き出して書いているのでこっちを見たほうが手っ取り早い（このことについて書籍ではきちんと説明できていない）
    * 逆にコードがあれば本は要らないのでこのリポジトリも作業を終わる
