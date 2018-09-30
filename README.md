# EZR 支付宝支付对接示例数据

- 1:条码支付下单
  [/alipay/open/createalipay](#) 
  ```js
  {
    "AppId": "EZP",
    "Timestamp": "1531969555",
    "Sign": "90d58312ab9bef88600c82111348cc6ed81c3713",
    "TradeNo": "WP01603818071800000011",
    "ShopCode": "5000001",
    "TotalAmount": 1.01,
    "AuthCode": "283955481090861617",
    "DiscountableAmount": 0,
    "UndiscountableAmount": 0,
    "GoodsDetail":[{"goods_id":"1304203","goods_name":"1毛测试商品","quantity":1,"price":"1"}],
    "Subject": "鞋子",
    "Body": "休闲鞋"
  }
  ```

- 2:订单信息查询接口 [/alipay/open/getorderinfo](#) 
  ```js
   {
    "AppId":"EZP",
    "TradeNo":"AP01322118093000000023", 
    "ShopCode":"5000001",
    "UserId":"", 
    "Sign":"b8057ae48db7528f235f8b7e52f5cc3f56bf423e"
  }
  ```

- 3:支付订单列表获取  [/alipay/open/getorderlis](#) 
  ```js
  {
    "AppId":"EZP", 
    "ShopCode":"5000001", 
    "TradeNo" : "AP063751517082400003193",
    "PageIndex":1,
    "PageSize":10, 
    "Sign":"4414758c5cdf8c0dfcb9268bf4c27249640097c4"
  }
  ```

- 4:退款申请接口 [/alipay/open/createalipayrefund](#) 
  ```js
  {
	"AppId":"EZP",
	"TradeNo":"AP01322118093000000023",  
	"RefundFee":100, 
	"Sign":"d19715109f1ed47f94d0ee00858cf892e75d9be6"
  } 
  ```

- 5:退款单列表查询 [/alipay/open/getorderrefundlist](#) 
  ```js
  {
    "AppId":"EZP",  
    "ShopCode":"5000001", 
    "PageIndex":1,
    "PageSize":20,
    "Sign":"45c2e68b97bb8fee232fc64d4ee5a8833569335e"
  }
  ```

- 6:支付订单取消接口 [/alipay/open/tradecancel](#) 
  ```js
  {
    "AppId":"EZP",
    "TradeNo":"AP01803518093000000020", 
    "ShopCode":"5000001",  
    "RefundFee":2,
    "GoodsDetail":[{"goods_id":"1304203","goods_name":"1毛测试商品","quantity":1,"price":"1"}],
    "Sign":"b9b851dedb14e200d9bf54019c6fa1a8738412b0"
  }
  ```
