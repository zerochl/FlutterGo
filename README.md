## 申明（Statement）
本项目与Google的Flutter没有任何关系，Flutter英文字面意思为震动，FlutterGo即为用Go来实现移动端的多平台共振。

This project has nothing to do with Google's flutter, which literally means vibration in English. Flutergo means using go to realize multi platform resonance of mobile terminal.
## 愿景(Vision)
实现类似Flutter的跨平台开发功能，超越Flutter，解决Flutter无法解决的各种兼容问题。

It realizes the cross platform development function similar to that of flutter, surpasses flutter and solves various compatibility problems that cannot be solved by flutter.
## 方案(Programme)
专业的事情交给专业的人来做，原生负责UI实现，GoLang包揽所有业务逻辑，整体按照MVP开发模式来进行。

Professional things should be done by professional people. The original UI implementation is responsible for. Golang takes charge of all business logic. The overall development mode is MVP.
## Google Flutter的优缺点(Advantages and disadvantages of Google fluent)
|        | Flutter |
| :----: |  :---- |
| 优点 | 1、使用全新的类似游戏开发的引擎来进行页面渲染，流畅性不错 |
| advantage | 1.Using a new engine similar to game development to render the page, good fluency |
|  | 2、可全部使用Flutter也可Native+Flutter结合，比较灵活 |
|  | 2.It can be used all flutter or native + flutter, which is more flexible |
|  | 3、动态编译运行速度快 |
|  | 3.Dynamic compilation runs fast |
| 缺点 | 1、万年长谈，兼容性不好 |
| disadvantages | 1.Long talk, poor compatibility |
|  | 2、生态不行 |
|  | 2.Ecology is not good |
|  | 3、风格与原生迥异 |
|  | 3.The style is quite different from the original |
|  | 4、内存占用过多 |
|  | 4.Too much memory |
|  | 5、耗电大 |
|  | 5.High power consumption |
|  | 6、UI绘制相当吃力 |
|  | 6.UI rendering is quite laborious |
## FlutterGo的优缺点（Advantages and disadvantages of flutergo）
|        | FlutterGo |
| :----: |  :---- |
| 优点 | 1、UI回归原生，控件没有任何坑 |
| advantages | 1.The UI returns to native, and the control has no holes |
|  | 2、Go语言生态不错，只实现业务逻辑毫无难度 |
|  | 2.Go language ecology is good, only the implementation of business logic is not difficult |
|  | 3、支持CPU密集型运算 |
|  | 3.Support CPU intensive computing |
|  | 4、上手容易 |
|  | 4.Easy to use |
| 缺点 | 1、需要原生绘制UI |
| disadvantages | 1.Need native rendering UI |
## 对比总结（Comparative summary）
总得来讲，让原生来实现UI是最正确的事，业务逻辑按照MVP开发模式使用GoLang来实现完全可取，期待各位的加入

Generally speaking, it is the most correct thing to let the native implement UI. It is entirely desirable to use golang to implement business logic according to MVP development mode. I look forward to your participation
## FlutterGo编译环境准备（Preparation of compiling environment for flutergo）
  1.准备GoLang环境（Prepare golang environment）
  
    请自行查阅相关文档
    Please refer to the relevant documents
    
  2.获取GoMobile源码（Get gomobile source code）
  
    go get golang.org/x/mobile/cmd/gomobile
    
  3.配置NDK环境变量（Configure NDK environment variables）：NDK_HOME
  
  4.初始化GoMobile（Initialize gomobile）
    
    gomobile init
    
  5.编译Android AAR包（Compile Android AAR package）
    
    进入go workspace即src文件夹下（Enter the go workspace, that is, the SRC folder）
    gomobile bind -target=android FlutterGo
    
  6.编译iOS Framework库（Compiling IOS Framework Library）
  
    进入go workspace即src文件夹下（Enter the go workspace, that is, the SRC folder）
    gomobile bind -target=ios FlutterGo
