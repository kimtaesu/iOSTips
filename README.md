# iOSTips


### lazy var 에서의 Closure 순환 참조가 발생하는 케이스와 발생하지 않는 케이스 정리
[Closuer 순환 참조](https://github.com/jinuman/TIL/blob/master/swift/swift-closure-retaincycle.md)

### iOS 앱 강제 종료?
[카카오톡방 YRH님]()
```
DispatchQueue.main.asyncAfter(deadline: .now() + 1.0) {
    UIApplication.shared.perform(#selector(NSXPCConnection.suspend))
     DispatchQueue.main.asyncAfter(deadline: .now() + 0.5) {
      exit(0)
     }
}
```

[closeAppElegantly.swift](https://gist.github.com/yoni-g/f6deb954ad31fef288662949bf7c9cbe)
앱 심사 거절 관련 Comment! 확인 필요!

### RxSwift 

#### switchLatest
map과 switchLatest을 합치면 flatMapLatest이다.
