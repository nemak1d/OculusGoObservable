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

# Requirement
* [Unity 2018.1.1f1](https://unity3d.com/jp/get-unity/download/archive)
* [Oculus Integration ver.1.25](https://assetstore.unity.com/packages/tools/integration/oculus-integration-82022?aid=1011lGbg&utm_source=aff)
* [UniRx](https://github.com/neuecc/UniRx)

