# 前言

欢迎来到我们的基于微信小程序的闲置品交易平台项目！在这个项目中，我们使用了Spring Boot技术，结合了微信小程序的前端优势，致力于为大家提供一个便捷、高效的闲置物品交易平台。以下是项目的详细介绍。

# 内容介绍

本项目是一个基于微信小程序的闲置品交易平台，用户可以在平台上发布自己的闲置物品，也可以浏览并购买其他人发布的闲置物品。平台提供了完善的商品管理、订单管理和用户管理功能，让用户能够轻松地进行交易。此外，我们还注重用户体验，提供了简洁明了的操作界面和流畅的交互体验。

# 技术介绍

## 语言：Java

## 使用框架：
- Spring
- Springmvc
- Mybatis
- 微信小程序

## 前端技术：
- JS
- Vue
- CSS3
- Uniapp

## 开发工具：
- IDEA/Eclipse
- Uniapp

## 数据库：
- MySQL 5.7/8.0

## 数据库管理工具：
- phpstudy/Navicat

## JDK版本：
- jdk1.8

## Maven：
- apache-maven 3.8.1-bin

## 前端环境：
- Node.Js 12\14\16

# 核心代码

以下是项目中的一部分核心代码，用于实现商品列表功能：

```java
// GoodsController.java
@RestController
@RequestMapping("/goods")
public class GoodsController {

    @Autowired
    private GoodsService goodsService;

    @GetMapping("/list")
    public ResponseEntity<List<Goods>> list(@RequestParam("page") int page,
                                           @RequestParam("size") int size) {
        Pageable pageable = PageRequest.of(page, size);
        List<Goods> goodsList = goodsService.findAll(pageable).getContent();
        return ResponseEntity.ok(goodsList);
    }
}
```

# 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图
## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
