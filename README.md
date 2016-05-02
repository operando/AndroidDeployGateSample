# AndroidDeployGateSample [![Build Status](https://travis-ci.org/operando/AndroidDeployGateSample.svg?branch=master)](https://travis-ci.org/operando/AndroidDeployGateSample)


## 概要

* DeployGate + Travis CIの構成
* Travis CIからmasterにコミットがあった場合に限りdebugアプリをDeployGateにあげる
* ローカル環境からDeployGateにあげる場合は`app/gradle.properties`にapi tokenを記載して実行する


## 参考

* [Travis CIを使ってgradleでDeployGateに自動デプロイ](http://qiita.com/hogelog/items/e24591cf9c2abac4712b)
* [Travis CIからDeployGateにアップロードする](http://henteko07.hatenablog.com/entry/2014/03/12/231851)
* [gradle-deploygate-plugin](https://github.com/DeployGate/gradle-deploygate-plugin)
* [Default Environment Variables](https://docs.travis-ci.com/user/environment-variables/#Default-Environment-Variables)
* [Travis CI 上の環境変数（PULL_REQUEST, BRANCH, TAG）を使って、ワークフローの改善とリリース自動化を実現する](http://qiita.com/yoheimuta/items/64b8bd51a8fa4cb1b57d#travis_pull_request)


## TODO

* ローカル環境でmaster branch以外から自分のタイミングでDeployGateにUpすることが頻繁にあるかどうか
 * 初期の開発や新機能の開発でMockを上げて見てほしいとかならニーズはある
 * ローカル環境からGradleでUpしないような運用にする場合、pluginの読み込みなどをCI環境だけに絞ればbuildが多少は早くなりそう
 * 気にするほど早くなりそうにはないけど...