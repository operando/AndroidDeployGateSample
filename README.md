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
