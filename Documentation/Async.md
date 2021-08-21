# 非同期処理

[TODO] 非同期処理の前に TableView か CollectionView を利用して複数の拠点の天気予報を表示できるようにするのはどうだろうか

非同期処理を扱ってみましょう。

Async ver  
```swift
static func asyncFetchWeather(_ jsonString: String, completion: @escaping (Result<String, YumemiWeatherError>) -> Void)
```
[APIの概要](YumemiWeather.md#async-ver)  

## 課題
- 呼び出しAPIを`Async ver`に変更する
- APIの処理が戻るまで各拠点の View に天気予報取得中の UI 表示を行う

※イメージ  
![async](Images/Async.gif)
