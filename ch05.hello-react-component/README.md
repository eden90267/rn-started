# Hello React Component!

## Component 與 React Element

### 聲明式定義 Component

- 用來產生 React Element 實體 (Virtual DOM 節點)
- 使用 JS 編寫，Component 本身足以完整表達其可能的顯示變化和行為
- 可以自由嵌套或組合，讓前端 UI 程式有更好的可組合性與可重用性
- 自定義封裝資料接口及功能接口
- Component Class 名稱首字母必須大寫 (大駝峰式 Upper Camel Case)
- 在元件的 render 方法中，return React Element 來呈現 UI 內容
- 每個 Component，render 中只能有一個根節點元素

## 註冊 React 進入點

```javascript
import {AppRegistry} from 'react-native';
// Root Component
class App extends Component {
  render() {
    return (
      <View style={styles.container}>
        <Text style={styles.welcome}>
          Welcome to React Native!
        </Text>
        <Text>Hello World</Text>
      </View>
    );
  }
}

AppRegistry.registerComponent('app_name', () => App);
```

## 可嵌套的巢狀組件 - 樂高的組合堆疊

```javascript
class Greeting extends Component {
  render() {
    return <Text>Hello {this.props.name}!</Text>
  }
}
```

```javascript
class LotsOfGreeting extends Component {
  render() {
    return (
      <View style={{alignItems: 'center'}}>
        <Greeting name="React" />
        <Greeting name="Native" />
        <Greeting name="JavaScript" />
      </View>
    )
  }
}
```

## JSX (React.createElement)

- JSX 是 React 在使用的一種特殊 JavaScript 語法糖
- 需要翻譯成原本 React.createElement 語法才能執行
- 能狗讓你以可讀性較高的語法來定義 React UI 結構

### 注意事項

- 嚴格的標籤閉合語法
- 擁有屬性參數
- 屬性名稱改成以小駝峰式命名

## JSX 的 JavaScript 表達式


