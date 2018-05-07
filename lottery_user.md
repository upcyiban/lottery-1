
#### /lottery/user

- /lottery/user/pass
      GET方法
    -　描述：　获取所有创建的抽奖
    - 参数：　Authorization
    - 返回　：{
       "code":1,
       "msg":"所有过的抽奖",
       "object":[
            {
                "id": id,
                "creatorid":id,
                "lotteryname":"抽奖的名字（几等奖）",
                "lotteryintro":"具体的奖品名字",
                "lotterytimebegin":"开始的时间",
                "lotterytimeend":"结束的时间",
                "createtime":"创建的时间",
                "ispass":1/0 ， //1就是该抽奖没问题。
                "passcode":123456  , //抽奖验证用的
                " feedback":"反馈信息",
                "feedbackTime":"反馈的时间"
               我的 "prizes":[
                                {
                                "id":id,
                                "creatorId":creator,
                                "prizeName":"nanf",
                                "prizeInfo":"info",
                                "prizePercentage":12121212,
                                "totalNumber":该奖项的名字
                                "lotteryId":抽奖的id
                                }
                                .
                                .

                ],
               获奖 "prizeLists":[
                    {
                            "id":id,
                            "lotteryid":id,
                            "yibanid":"id",
                            "yibanname":"真实名字",
                            "prizeName":"几等奖",
                            "prizeStage":"具体的奖品名字";
                    },
                    {


                            "id":id,
                            "lotteryid":id,
                            "yibanid":"id",
                            "yibanname":"真实名字",
                            "prizeName":"几等奖",
                            "prizeStage":"具体的奖品名字";
                    }
                ]
                .
                .
            },
            {
                "id": id,
                "creatorid":id,
                "lotteryname":"抽奖的名字（几等奖）",
                "lotteryintro":"具体的奖品名字",
                "lotterytimebegin":"开始的时间",
                "lotterytimeend":"结束的时间",
                .
                .
            }....
        ]
        }
    
- /lottery/user/notPass
   GET 请求
   授权的token
   
 返回值：
   
- /lottery/user/warning 

post方法

- Authorization
- long lotteryId
- String feedback
- 描述　：　用户发现抽奖不好，进行举报的接口。
- 返回　：{
    "code":1,
    "msg":"举报成功",
    "object":null
}
   http://localhost:6060/?verify_request=c21f263641f5b94c0b20f9ec5d2ad13f7e94ed5c3e72a019983a2afbdbd1e8dc40d321d41e711fa66e569a784c10914d5ae9ec50233371887bc5dff9075493f6bca5fe4064ad2955942e76c1bfcf535415fa17d171a35303dcab1b54d01a6033d382ff895f2283af5f4aed9934c88aa8af6ecdf2b446c8d2055209ac90d2ad8cd3c90cf292475993565590bc6e11836800e362baa8e27be1bd92c3afe0716ad3018f7c7ca31e76c78d34cbc00c6cd5e305bca84412a2449b3818191b64e836022bf62a105ec35914d7038d1cceef330cb38b41b1415d699b20b42e5d5bfb706b&yb_uid=8671077&state=undefined

   http://localhost:6060/?verify_request=c21f263641f5b94c0b20f9ec5d2ad13f6d76da4910cd1ba6a3e1dbe870bf4fb33fa7b5d8b2be6fe10de662b159df9c3ce152857c262dfe8159392d3469edcb6df64990cdf7b331880d342177669d91b5921fb3258787719aa36a9083d005c3095ec4887db67ec603591cf46b39e99aef471ec13229f05f178798456cdadc24a4c75ac7dea12a1cfa6aec73bfd04d41831bc23d00a5c91bfe4ee45b948b6469136d66ef806f2860375e658ad61dfbe0ed22012ecd895877d3a08ea8b788f9c43b8e25b15e6558897241bd758956001e6f4340f26f25af56c3457147cf1d700db2&yb_uid=8671077&state=5050

   http://localhost:6060/?verify_request=c21f263641f5b94c0b20f9ec5d2ad13f246f9d11276ab2d83658f45228fab7e0941d77d39d888c26bb590da0399d2970cf3e8976c332d5691fb9685e659c7af65d513c3cd9d6911f93a15d4b4451f58a4428a1678b3cc96b6e6837a58c7fb9d151bca6690cac00110e1e8fe6b7cce3e28e58263ab9224a243cb361b81ccf7693cf6dc58fc49acc1a35eed38817418be8bc77b0b6b981a0a1ce0cbb1ab00c6c8508ab4a37dd8bd3617dfe572f35e66b672a10fe3329fed2ed04f3f695e7a03e54ae1a98f176a2d0438b66d1792a9e28cad273a167d33860db8cd28bf5bf19c0df&yb_uid=8671077&state=undefined


   http://localhost:6060/load.html?verify_request=c4e43f07625c459bd3fedec9c&yb_uid=5394432&state=5050