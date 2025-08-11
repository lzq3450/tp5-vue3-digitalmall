# tp5-vue3-digitalmall
数码商城基于前后端分离,前端vue3,后端tp5
# 数码商城
数码商城项目(买家方)
## 前端vue3+vite+nodejs,后端thinkphp5,数据库为mysql
### 从2025.8.1到2025.8.11完结撒花
## 端口
+ 前端5173
+ 后端8080
## 前端启动
1. npm run dev
## 前端测试登录
+ username:admin
+ password:111111
## 技术栈

+ 前端：vue3 + vue-router + vuex + nodejs + Element-plus + axios + vueuse

+ 后端：thinkphp5、mysql

## 功能
1. 实现了基本的CRUD、商品分类显示、购物车显示、支付
2. 物品搜索功能，以及翻页功能，以及点击查看物品详细信息
3. 对物品进行下单、加入购物车,填写收货地址以及电话，以及表单验证收货地址和电话不为空
4. 实现登录注册功能，未登录的用户不能查看购物车，下单，订单，个人信息。
5. 对于已经登录的用户可以进行修改密码，修改密码的前提得进行旧密码验证。
6. 对于订单，订单可以删除。
7. 对于购物车，购物车可以支付，可以修改购买数量，可以移出购物车。

### 作者:

szpu,大数据专业lzq开源

## 数据库ashuma

1. goods (商品表)
+ id 商品ID
+ name 商品名称
+ price 商品价格
+ pic 商品图片
+ note 商品补充说明

2. tb_order (订单表)
+ id 订单ID
+ user_id 用户id
+ goods_id 商品ID
+ order_sn 订单号
+ goods_num 购买数量
+ goods_prices 商品价格
+ order_money 订单总价
+ phone 手机号
+ address 地址
+ createtime 订单创建时间
+ updatetime 更新时间

3. tb_shopcar
+ id 序号
+ user_id 用户id
+ goods_id 商品ID
+ goods_num 购买数量

4. user (用户表)
+ id 用户id
+ username 用户名
+ password 用户密码
+ createtime 创建时间
+ updatetime 更新时间
