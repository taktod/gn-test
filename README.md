# gnやってみた。

# 作者

taktod
https://twitter.com/taktod

# 概要

とりあえずgnで適当なプロジェクトをつくってみたかった。

# ベース

まんまこれ
https://blog.simplypatrick.com/posts/2016/01-23-gn/
ただしtoolchainのとこがうまく動作しなかったので、ちょっとだけ書き換えた。

# 使い方

https://github.com/nodejs/node/issues/6089
ここのtojockyさんのコメントにあるstandaloneで動作するgnを作らなければいけない。

とりあえずスクリプトいれといたので、実行する。

```
$ ./build-gn.sh
```

するとgn-standalone/out/Release/gnができる。

```
$ gn-standalone/out/Release/gn gen out
$ ninja -C out
$ out/hello
```

これでhello world!と出力される実行プログラムができてるはず。

OSXで確認しました

# ライセンス

MIT
