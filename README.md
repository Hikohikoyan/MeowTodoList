# MeowTodo

![](https://github.com/Hikohikoyan/MeowTodoList/blob/master/miniprogram/images/todoicon.png)

主页功能：微信登录+获取全部事件列表 并按优先级（距离ddl时间-->紧急程度-->重要程度--->添加时间）返回数组，返回errmsg和errcode

录音功能：长按调用微信录音和语音转写api 点击添加时 自动塞入事件列表 并返回errmsg和errcode

## 前后端文档接口说明

baseurl: [后端填写]

### 主页 index

1.获取list GET请求

请求地址：api/ [后端填写] 

后台返回todo的内容格式如下：（json

```json
    todo: [{
      item: {
        index:1,
        name:'计网实验',
        time:'2020/3/24',
        msg:'距离截止日期只剩下3天了！',
        group:'分组1',
        important:6//星级 返回星星个数
      },
    }, {
      item: {
        index:2,
        name:'计网实验',
        time:'2020/3/24',
        msg:'',
        group:'分组2',
        important:3
      },
      
    }, {
      item: {
        index:3,
        name:'实验',
        time:'2020/3/24',
        msg:'备注：要去实验室',
        group:'分组2',
        important:2
      },
      
    }, {
      item: {
        index:4,
        name:'验',
        time:'2020/3/24',
        msg:'',
        group:'分组2',
        important:5
      },
      
    }, {
      item: {
        index:5,
        name:'验',
        time:'2020/3/24',
        msg:'',
        group:'分组2',
        important:5
      },
      ......
    }]
```



### 云开发 quickstart

这是云开发的快速启动指引，其中演示了如何上手使用云开发的三大基础能力：

- 数据库：一个既可在小程序前端操作，也能在云函数中读写的 JSON 文档型数据库
- 文件存储：在小程序前端直接上传/下载云端文件，在云开发控制台可视化管理
- 云函数：在云端运行的代码，微信私有协议天然鉴权，开发者只需编写业务逻辑代码

### 参考文档

- [云开发文档](https://developers.weixin.qq.com/miniprogram/dev/wxcloud/basis/getting-started.html)

