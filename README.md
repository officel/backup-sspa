# Learning Serverless Single Page Apps

## memo

* 日本語版サーバレスシングルページアプリケーション本（オライリー）の写経
* オリジナルは [benrady/learnjs: Prepared Workspace for "Serverless Single Page Apps" @ Pragprog](https://github.com/benrady/learnjs)

    * 若干中身が古いので少し変更
    * [necolas/normalize.css: A collection of HTML element and attribute style-normalizations](https://github.com/necolas/normalize.css/) を 7.0.0 に
    * [jQuery](http://jquery.com/) を 3.2.1 に
    * [dhg/Skeleton: Skeleton: A Dead Simple, Responsive Boilerplate for Mobile-Friendly Development](https://github.com/dhg/Skeleton/) は3年前で更新停止しているようだ
    * オリジナルの vendor.js の中の AWS SDK は導入の仕方が不明瞭なのとどうせすでに使い物にならないくらい古いはずなので使う段階になったら入れる

        * インストールされているはずなのは以下のとおり
        * CognitoIdentity
        * CognitoSync
        * DynamoDB
        * Lambda
        * STS

