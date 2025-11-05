## 前言

此项目为基于SpringBoot+Vue的疫情物资捐赠和分配系统，是我毕业设计的实战项目。项目利用Java语言开发，采用Spring Boot框架，前端使用JS、Vue及CSS3技术，数据库选用MySQL 5.7/8.0。以下为项目的详细介绍。

## 内容介绍

本项目旨在为疫情期间的物资捐赠和分配提供便捷、高效的解决方案。系统主要包括以下几个功能模块：用户管理、物资管理、捐赠管理、分配管理等。用户可以通过系统实时查看物资库存情况，进行物资捐赠和申请，管理员则可以对捐赠物资进行分配和管理。

## 技术介绍

- 语言：Java
- 使用框架：Spring Boot
- 前端技术：JS、Vue、CSS3
- 开发工具：IDEA/Eclipse
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven: apache-maven 3.8.1-bin
- 前端环境：Node.Js 12\14\16

## 核心代码

以下为物资管理模块的部分核心代码：

```java
@RestController
@RequestMapping("/material")
public class MaterialController {

    @Autowired
    private MaterialService materialService;

    @GetMapping("/list")
    public Result list(MaterialQuery materialQuery) {
        Page<Material> page = materialService.findMaterialByPage(materialQuery);
        return new Result(true, page);
    }

    @PostMapping("/add")
    public Result add(@RequestBody Material material) {
        materialService.saveMaterial(material);
        return new Result(true, "添加成功！");
    }

    // 其他接口...
}
```

## 免费源码获取

```
8000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img10.360buyimg.com/ddimg/jfs/t1/316341/11/25360/188722/689ead0cF2e520418/859bf932c1e3cf76.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/326421/23/4762/45466/689eacebF7a4eb0a9/e5f2ab16925577e6.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/324309/36/4670/130875/689eacecF5f952f14/06082f934ea77484.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/310114/7/26921/36095/689eacedF82db3fd0/096d63f0185c429b.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/326090/3/4755/51466/689eacedFad733f58/cac592541545dbe8.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/310208/24/26480/78474/689eaceeF2f5c3a0a/09ded78e927ddd5e.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/294956/40/19436/75500/689eacefFb2d990c4/31b56c3b14c2075c.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/318172/1/24911/44012/689eacefF912d217b/df1129d4c7ef7e87.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/312425/31/26701/31616/689eacf0F210233c7/ad42b6d5b8787d64.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/324138/1/4778/58874/689eacf0F6d8dd67c/7cad5b63f39d744a.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
