# 设计

## 流程

![Flow](img/flow.jpeg)

## 微信菜单设计

![1](img/2.png)

- 首页
- 分类选购
  - 精选
  - 鲜花
  - 花园
  - 超度
- 我
  - 我的订单
  - 心情

## 详细分类菜单

![1](img/5.png)

- 精选
  - 蝴蝶花
    - 2016《里》-》详情页
- 鲜花
  - 四季歌
    - 春 -》分类列表
    - 夏 -》分类列表
    - 秋 -》分类列表
    - 冬 -》分类列表
- 花园
  - 居所 -》分类列表
  - 记忆 -》分类列表
  - 记烧 -》分类列表
  - 光音 -》分类列表
  - 折思 -》分类列表
  - 其他 -》分类列表
- 超度
  - 佛 -》分类列表
  - 道 -》分类列表

结论

- 分类最多3级
- 分类可以帮到分类列表也或详情页

添加的商品和分类有绑定

## 分类列表页

默认分类菜单页面

![1](img/3.png)

步骤拆分

- 点击菜单按钮，弹出分类菜单
- 默认显示【精选】-》蝴蝶花2016
- 点击2016《里》进入具体详情，此时可以加入购物车
- 点击头部的【我的购物车】按钮，进入购物车
- 在购物车页面结算（含支付），生成订单
- 点击头部的【我的】按钮，进入个人中心，可以查看我的订单

选中【鲜花】分类，切换【四季歌】列表，点击【春】进入到分类列表页

![1](img/4.png)

说明

- 分类列表页有4个筛选，排序按钮
  - 年（筛选）
    - 0~1
    - 1~5
    - 5~10
    - 10+
  - 综合（排序）
  - 销量（排序）
  - 价格（排序）

## cell

![Cell](img/cell.png)

- 商品名称
- 商品描述
- 价格
- 年份

## 详情页

- detail

![D1](img/d1.png)

- 商品名称 + 价格￥15.00
- 头图（数组）
- 所属菜单（春）
- 所属分类（年份：0~1年）
- 备注（* 7 天无理由退货，15 天免费换货，满 150 元免运费。）
- 加入购物车

![D2](img/d2.png)

- 商品详情（图文）

推导出商品模型

- 商品名称 
- 销量（分类列表-排序）
- 价格￥15.00（分类列表-排序）
- 头图（数组）
- 所属菜单（春）
- 所属分类（年份：0~1年）
- 备注（* 7 天无理由退货，15 天免费换货，满 150 元免运费。）
- 创建时间
- 更新时间

状态

- 是否显示
- 是否首页
- 是否头图
- 是否推荐

## 首页

原型

![1](img/2.png)

- 置顶轮播，点击进入详情
- 头图推荐：比如超度，点击进入分类列表
- 当季
- 四季歌
  - 春，点击进入分类列表
  - 夏，点击进入分类列表
  - 秋，点击进入分类列表
  - 冬，点击进入分类列表
- 花园商品，点击进入花园分类列表
- 最下面：网站说明

参考

![1](img/index.png)

