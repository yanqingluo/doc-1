
### 重仓持股_QDII

**URL**

/f10/fund/zccg_qdii

**描述**

重仓持股_QDII

**参数说明**

|名称|类型|说明|缺省|
| -------- | -------- | -------- | -------- |
|obj\*|字符串|查询股票\*表示必填，必填的字段说明放在前面。如SH600000|无|
|field|字符串|字段以逗号间隔，为空则返回结构所有字段,关注字段以逗号分隔(见返回说明)|无|
|start|整型|行筛选，表示从以上步骤产生的数据的第几行开始往后筛选|无|
|count|整型|行筛选，大于等于0的整数，表示从start的位置往后筛选多少行数据（包括start），0或者空表示之后的所有行|无|


**结果说明**

```json
{
        "Id": 207,
        "RepDataF10FundZccgQdiiOutput": [
            {
                "Obj": "OF050025",
                "Data": [
                    {
                        "jzrq": "2013-09-30 00:00:00",
                        "data": [
                            {
                                "gpdm": "AAPL US",	// 股票代码	varchar(20)
                                "gpjc": "APPLE INC",// 股票简称	varchar(200)
                                "sl": 0.178,		// 数量（万股）	numeric(19,3)
                                "sz": 521.43,		// 市值（万元）	numeric(19,2)
                                "zjzb": 2.71		// 占净值比（%）	numeric(19,2)
                            }
                        ]
                    }
				]
			}
   	 	]
}
```

**示例**

[http://10.15.144.101/f10/fund/zccg_qdii?obj=OF050025]
获取OF050025的重仓持股_QDII  
