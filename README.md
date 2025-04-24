# SharpDdddOcr
DdddOcr的C#实现版本

原项目地址： [点我传送](https://github.com/sml2h3/ddddocr) 

### 项目底层支持 

本项目是[ddddocr](https://github.com/sml2h3/ddddocr)的C#实现，因为跨语言调用太麻烦了，所以直接转成了C#，仅实现了dddocr最基础的识别验证码
测试单线程识别100张验证码耗时1.2秒左右，因个人能力限制，代码质量低且短期内可能不会优化，请谅解

### 使用文档
```csharp
var ddddOcr = new DdddOcr();
var image = File.ReadAllBytes("example.jpg");
var result = ddddOcr.Classification(image);
Console.WriteLine(result);
```
