# Hi, React Native

## React Native 與其他移動設備應用開發方式的比較

| Web                                                                 | Hybrid                                                                                              | Cross-Platform Native                                      | Native                                            |
|:--------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------|:-----------------------------------------------------------|:--------------------------------------------------|
| <ul><li>HTML + CSS</li><li>JavaScript</li><li>Browser API</li></ul> | <ul><li>WebView</li><li>JSBridge</li><li>Native API</li><li>HTML + CSS</li><li>JavaScript</li></ul> | <ul><li>Native UX</li></ul>                                | <ul><li>Native UX</li></ul>                       |
| <ul><li>SPA</li><li>React</li><li>Vue</li></ul>                     | <ul><li><PhoneGap/li><li>Cordova</li><li>Ionic</li></ul>                                            | <ul><li>ReactNative</li><li>Weex</li><li>Xamarin</li></ul> | <ul><li>Swift</li><li>Java</li><li>.NET</li></ul> |

```
跨平台性 <---------------------------------------------> 使用體驗
```

## React Native 特點

- 跨平台，寫一份程式碼在不同平台運行
- 共享 React 生態圈的豐富資源
- 和 Web 開發流程相似，前端開發者容易入門
- 模組化及重用性 (facebook 團隊程式碼重用率 85%)
- 開發速度比傳統原生開發更快
- 相較 Hybrid 效能更高，體驗更好
- Hot Reloading 帶來良好開發體驗
- Hot Deploy，即時更新架上 App，快速迭代產品
- 具備 Native Module 擴充性
- 開發除錯工具整合完整

### 特別提醒

- 過舊版本不支援
  - Android >= 4.1 (API 16)
  - iOS >= 8.0
- 不會原生開發的話，就必須依賴官方或第三方套件支援
- Android 上目前樣式效果支援程度還差一些