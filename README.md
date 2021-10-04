# IntelliJ IDEA tips
IntelliJ IDEA に関する TIPS

## コンパイルエラー発生した状態で実行する方法

実プロジェクトでは、他者が作成したコードのコンパイルエラーが発生している状態で、自分のテストコードを実行したい状況がある。

1. `Save Actions` プラグインをインストールする
1. `File > Settings > Other Settings > Save Actions` に移動する
    1. `Activate save actions on save (before saving each file, performs the configured action below)` にチェックを入れる
    1. `[experimental] Compile files (using "Build > Build Project")` にチェックを入れる
1. 実行対象クラスの `Configurations` を開く
    1. `Run` の `Modify options > Do not build before run` にチェックを入れる

ファイル保存時に編集クラスのビルドが行われ、実行時ビルドが走らないのでコンパイルエラーが含まれていても実行可能となる。
