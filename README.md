## 百度翻译接口代码

### 代码流程
- 先从网页源码获取`gtk`和`token`这两个参数
- 执行生成`sign`的js代码，参数为`gtk`和`query_str(即要翻译的文本)`
- `sign`和`token`皆为提交数据时使用,利用这几个参数来构造请求的数据

### 使用流程
- 先打开[百度翻译](https://fanyi.baidu.com/),利用开发者工具，复制请求的cookie，
替换掉代码中的所有cookie
- 然后直接运行代码即可

### 注意事项
- `token`的生成依赖于你的cookie，所以请务必更换成自己的值