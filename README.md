# iOSTips

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
