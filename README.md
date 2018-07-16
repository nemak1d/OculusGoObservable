# OculusGoObservable
OculusGoコントローラ向けストリームソースラッパーです。  
Stream source wrapper for Oculus Go Controller.

# Description
コントローラの各ボタンに対する、  
* 入力時(OnTrigger)
* 入力中(OnPressing)
* 解放時(OnRelease)  

のタイミングに対応したストリームソースを提供します。  
また、タッチパッドをタッチしている最中にタッチ位置を通知するストリームソースを提供しています。

Provide stream source corresponding to  
* OnTrigger
* OnPressing
* OnRelease

and  
* Position of TouchPad at touch

for Oculus Go Controller.  

# Demo
e.g.)コントローラの引き金の入力時イベントは以下の通り記述します.  
e.g.)Input event on trigger of controller is write as follows.

```
OculusGoObservable.Instance.PrimaryIndexTriggerOnPressing
                .Subscribe(_ => Debug.Log("subscribe!"))
                .AddTo(this);
```


# Requirement
* [Unity 2018.1.1f1](https://unity3d.com/jp/get-unity/download/archive)
* [Oculus Integration ver.1.25](https://assetstore.unity.com/packages/tools/integration/oculus-integration-82022?aid=1011lGbg&utm_source=aff)
* [UniRx ver6.0.0](https://github.com/neuecc/UniRx)

# Installation
[UnityPackage](https://github.com/nemak1d/OculusGoObservable/blob/master/OculusGoObservable_v100.unitypackage)をインポートします  
Import the [UnityPackage](https://github.com/nemak1d/OculusGoObservable/blob/master/OculusGoObservable_v100.unitypackage).

# License
本リポジトリにおけるソースコードについては原則Public Domainを適用します。  
ただし、UniRxにおけるライセンスは別途適用されている必要があります。  
Copyright (c) 2014 Yoshifumi Kawai https://github.com/neuecc/UniRx/blob/master/LICENSE
