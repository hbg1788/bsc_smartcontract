#HBG智能合约3.0写入BSC链解读及操作流程
- 第一、HBG理念和信仰不会改变，坚定不移的推广“垃圾分类”，为建设更多美丽富饶的“卫生文明城市”添砖加瓦，HBG没有“套路”，共识决定未来
- 第二、HBG质押挖矿用defi去中心化金融，把第三方彻底取代，将执行智能合约的代码写在BSC链上，而非托管。公开的开源挖矿代码与BSC链共存，安全、可靠、有保障
- 第三、奖励机制，推荐会员质押挖矿，可以获得该会员质押收益的10%作为奖励，奖励只有1代
    
        HBG质押挖矿收益表
                        a                 b                 c              d
            30天   10.5            106           1070        5400
            60天   11.1             113           1150       5850
            90天   11.8             120           1240       6350
          180天   14.6             152           1580       8100

#####a代表10HBG    b代表100HBG    c代表1000HBG    d代表5000HBG 
#####a30表示：10HBG质押30天.....依此类推....d180表示：5000HBG质押180天
HBG合约地址：[0x1a01FaEC8E52756c09A33c5b06d3b58727c0c0cc](https://bscscan.com/token/0x1a01FaEC8E52756c09A33c5b06d3b58727c0c0cc "0x1a01FaEC8E52756c09A33c5b06d3b58727c0c0cc")
HBG质押地址：
[0x073e86e3c6f9a71B1B02f8eD2D6F707dCF0A8BD1](https://bscscan.com/address/0x073e86e3c6f9a71b1b02f8ed2d6f707dcf0a8bd1#readContract "0x073e86e3c6f9a71B1B02f8eD2D6F707dCF0A8BD1")

    HBGT质押挖矿收益表
                   a               b                c                  d
    30天    105           1060         5350          10800
    60天    111            1130        5750          11700
    90天    118            1200         6200          12700
    180天  146            1520         7900          16200
#####a代表100HBGT    b代表1000HBGT    c代表5000HBGT     d代表10000HBGT
#####a30表示：100HBGT质押30天......依此类推......d180表示：10000HBGT质押180天
HBGT合约地址：[0xFF2904DAcf60D9cc275068D588d85FA1F28696F1](https://bscscan.com/token/0xFF2904DAcf60D9cc275068D588d85FA1F28696F1 "0xFF2904DAcf60D9cc275068D588d85FA1F28696F1")
HBGT质押地址：[0x1802C3e0cf1EC469a01c5A4dc9951bde8d059fed](https://bscscan.com/address/0x1802C3e0cf1EC469a01c5A4dc9951bde8d059fed#readContract "0x1802C3e0cf1EC469a01c5A4dc9951bde8d059fed")

#质押挖矿流程：
- 第一步 链接钱包：打开tp钱包——发现——在搜索栏输入币安链网址bsccan.com——在币安链搜索栏输入质押合约地址——点击contract——点击Write写入——点击connect to web3链接钱包——选择walletconnect确认——选择TP钱包确认授权——链接成功红点会变成绿点
- 第二步质押挖矿：
- 1.Bindlnviter绑定推荐人——输入推荐人的钱包地址即可
注意：
	1. 只有一次绑定的机会，不可以修改
	2. 不可以A推荐B，B推荐A循环推荐 
	3. 领导人必须是质押挖矿的会员，才可以拿到收益

2.Pledging 质押挖矿——先计算自己钱包的余额输入挖矿代码例如：a30…b60…c90…d180——提交——操作完成✅（字母都是小写abcd…）

第三步质押赎回：
3.RedeemPledge到期赎回——直接点击Write赎回即可

4.WithdrawBonus领导人奖励领取——直推会员完成质押赎回以后，直接点击Write领取即可

（温馨提示：1.随着社区布道者共识的增多，质押挖矿总量的增加，市场可流通的数量减少，价格随之上涨  2.walletconnetc如果链接的时间过长，会导致登入失效，点击下方Reset退出重新连接即可    3.BSC链上操作的过程需要少量的bnb作为手续费  4.转入黑洞获取BSC链资产时间为7月10日0时—7月15日0时（切记上链数据一定要填写正确的BSC链钱包地址）  5.从2022年7月10日开始，每年7月10日减产一次，减产收益由社区投票决定，提前一个月公布 ）

查询全网数据教程（选学）：
第一步链接钱包：打开币安链网址bsccan.com——在币安链搜索栏输入质押合约地址——点击contract——点击Read阅读
1.GetpledgePlanlnfo查询全网质押数据例如：输入代码a30——amoumt：显示数量去掉6个0，为全网a30质押的总量——day：为天数——rare：显示数字去掉4个0，为a30收益百分比——bonus：显示数字去掉4个0，为领导人收益百分比
2.GetPledgePlans 代码编号3.GetRedeemable、4.GetUserlnfo、5.GetUserPledages3.4.5均为个人信息
6.owner：合约账户
7.sumPledgingAmount：全网质押总量
