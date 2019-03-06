# Quotes

收集了一些每日一句的接口与网站。

iOS 捷径：[每日一句](https://www.icloud.com/shortcuts/6bb4e30a50584ddb8e791930f1e9f3be)

## 接口集合

[Postman share link](https://www.getpostman.com/collections/98d52280966545820fe4)

### ONE

- API：https://api.hibai.cn/api/index/index
- 请求方法：POST
- 调性：小众，文艺
- 类型：图文

#### 请求参数

Post form-data

| 属性名    | 默认值 | 必填 | 说明                                   |
| --------- | ------ | ---- | -------------------------------------- |
| TransCode |        | 是   | 030111：当天数据，030112：最近一周数据 |
| OpenId    |        | 是   | 随便填，保证字段非空即可               | --- |

#### 返回值

```
{
    "ResultCode": 1,
    "ErrCode": "OK",
    "Body": {
        "id": 5065,
        "vol": "VOL.2342",
        "img_url": "http://image.wufazhuce.com/Fj7zpzj6kuRpJtElqwUkExkDqKUq",
        "img_author": "徐盛哲",
        "img_kind": "摄影",
        "date": "2019-03-06 06:00:00",
        "url": "http://m.wufazhuce.com/one/2372",
        "word": "曾经爱你的每一条街，是我新鲜生活的起点 。",
        "word_from": "李志",
        "word_id": 2372
    }
}
```

### 金山词霸

- API：http://open.iciba.com/dsapi/
- 请求方法：GET
- 文档：http://open.iciba.com/?c=wiki
- 调性：励志，鸡汤
- 类型：图文

#### 请求参数

| 属性名 | 默认值   | 必填 | 说明                                              |
| ------ | -------- | ---- | ------------------------------------------------- |
| file   | json     | 否   | 数据格式，默认 json，可选 xml                     |
| date   | 当前日期 | 否   | yyyy-MM-dd，默认当前日期                          |
| type   |          | 否   | date 日期为基准，last 返回前一天，next 返回后一天 |

#### 返回值

需要 JSON 解码

```
{
    "sid": "3318",
    "tts": "http://news.iciba.com/admin/tts/2019-03-06-day1.mp3",
    "content": "Try to be a rainbow in someone’s cloud. ",
    "note": "努力成为别人乌云里的一道彩虹。",
    "love": "1215",
    "translation": "小编的话：当雨过天晴时，太阳照在云雨之中，你就是那天边的一抹彩色的虹，自然、纯净，美不胜收。",
    "picture": "http://cdn.iciba.com/news/word/20190306.jpg",
    "picture2": "http://cdn.iciba.com/news/word/big_20190306b.jpg",
    "caption": "词霸每日一句",
    "dateline": "2019-03-06",
    "s_pv": "0",
    "sp_pv": "0",
    "tags": [
        {
            "id": null,
            "name": null
        }
    ],
    "fenxiang_img": "http://cdn.iciba.com/web/news/longweibo/imag/2019-03-06.jpg"
}
```

### 扇贝

- API：https://api.tecchen.xyz/api/quote/
- 请求方法：GET
- 调性：励志，鸡汤
- 类型：图文

#### 返回值

```
{
    "code": 0,
    "message": "成功",
    "data": {
        "id": "bqtss",
        "author": "《蝙蝠侠：黑暗骑士》",
        "content": "The night is darkest just before the dawn. And I promise you, the dawn is coming.",
        "assignDate": "2019-03-06",
        "adUrl": null,
        "shareUrl": "https://www.shanbay.com/soup/mobile/quote/2019-03-06/",
        "shareUrls": {
            "weibo": "https://www.shanbay.com/soup/mobile/quote/2019-03-06/",
            "shanbay": "https://www.shanbay.com/soup/mobile/quote/2019-03-06/",
            "wechat": "https://www.shanbay.com/soup/mobile/quote/2019-03-06/",
            "qzone": "https://www.shanbay.com/soup/mobile/quote/2019-03-06/",
            "wechat_user": "https://www.shanbay.com/soup/mobile/quote/2019-03-06/"
        },
        "trackObject": {
            "code": "abb22",
            "share_url": "https://www.shanbay.com/soup/mobile/quote/2019-03-06/",
            "object_id": 2528
        },
        "translation": "黎明前的夜最黑暗。我向你们保证，黎明就要来到。",
        "originImgUrls": [
            "https://media-image1.baydn.com/soup_pub_image/ccdbwr/c8da96fd69d9d53a0a995945b54f192d.6ae4029909d0e049b396381a5e53a5f6.png",
            "https://media-image1.qiniu.baydn.com/soup_pub_image/ccdbwr/c8da96fd69d9d53a0a995945b54f192d.6ae4029909d0e049b396381a5e53a5f6.png?imageView2/2/w/1080/format/webp"
        ],
        "shareImgUrls": [
            "https://media-image1.baydn.com/soup_pub_image/hcmuf/9ffabf03e3f5a09058b0843f12e88faa.988d4a7565f4aae4af6e6bac720350bb.png@!w720",
            "https://media-image1.qiniu.baydn.com/soup_pub_image/hcmuf/9ffabf03e3f5a09058b0843f12e88faa.988d4a7565f4aae4af6e6bac720350bb.png?imageView2/2/w/720/"
        ]
    }
}
```

### 一言

- API：https://v1.hitokoto.cn/
- 请求方法：GET
- 官网：https://hitokoto.cn/
- 文档：https://hitokoto.cn/api
- 调性：二次元，网络，中二
- 类型：文字

#### 请求参数

| 属性名   | 默认值   | 必填 | 说明                                                          |
| -------- | -------- | ---- | ------------------------------------------------------------- |
| c        | 随机     | 否   | a: 动画, b: 漫画, c: 游戏, d: 小说, e: 原创, f: 网络, g: 其他 |
| encode   | json     | 否   | 可选值：text, json, js，当指定 js 时返回 jsonp                |
| charset  | utf-8    | 否   | 可选值：utf-8, gbk                                            |
| callback | hitokoto | 否   | jsonp 函数名，与 encode: js 配合使用                          |

#### 返回值

```
{
    "id": 4109,
    "hitokoto": "世界是无情的，并不存在与生俱来的英雄。 所以只能由刚好在旁边的人粉墨登场， 演一出英雄的戏码。",
    "type": "a",
    "from": "魔法禁书目录",
    "creator": "Amadeus",
    "created_at": "1540111436"
}
```

### 今日诗词

- API：https://v2.jinrishici.com/one.json
- 请求方法：GET
- 官网：https://www.jinrishici.com/
- 文档：https://www.jinrishici.com/doc/
- 调性：诗词，古风
- 类型：文字

#### 返回值

```
{
    "status": "success",
    "data": {
        "id": "5b8b9572e116fb3714e6fe94",
        "content": "桃花尽日随流水，洞在清溪何处边。",
        "popularity": 694000,
        "origin": {
            "title": "桃花溪",
            "dynasty": "唐代",
            "author": "张旭",
            "content": [
                "隐隐飞桥隔野烟，石矶西畔问渔船。",
                "桃花尽日随流水，洞在清溪何处边。"
            ],
            "translate": null
        },
        "matchTags": [
            "白天",
            "桃花"
        ],
        "recommendedReason": "",
        "cacheAt": "2019-03-06T16:46:48.003082"
    },
    "token": "1L+kOwPjxE0+1mtlehoED8XuDj11JncZ",
    "ipAddress": "61.135.152.135",
    "warning": null
}
```

### Storm

- API：http://quotes.stormconsultancy.co.uk/random.json
- 请求方法：GET
- 官网：http://quotes.stormconsultancy.co.uk/
- 文档：http://quotes.stormconsultancy.co.uk/api
- 调性：计算机，编程领域
- 类型：文字

#### 返回值

```
{
    "author": "E. W. Dijkstra",
    "id": 14,
    "quote": "If debugging is the process of removing software bugs, then programming must be the process of putting them in.",
    "permalink": "http://quotes.stormconsultancy.co.uk/quotes/14"
}
```

### Github

- API：https://api.github.com/zen
- 请求方法：GET
- 调性：启发，哲学
- 类型：文字

#### 返回值

```
Keep it logically awesome.
```

全部数据：https://gist.github.com/sorrycc/7214622

> "It's not fully shipped until it's fast."
> "Practicality beats purity."
> "Avoid administrative distraction."
> "Mind your words, they are important."
> "Non-blocking is better than blocking."
> "Design for failure."
> "Half measures are as bad as nothing at all."
> "Favor focus over features."
> "Approachable is better than simple."
> "Encourage flow."
> "Anything added dilutes everything else."
> "Speak like a human."
> "Responsive is better than fast."
> "Keep it logically awesome."

## 编程领域

### 网站

- http://www.defprogramming.com
- https://skolakoda.org/programming-quotes/#/
- http://quotes.stormconsultancy.co.uk/
- https://en.wikiquote.org/w/api.php
- https://www.goodreads.com/quotes/tag/programming
- https://www.brainyquote.com/topics/programming

### laravel inspire

https://github.com/laravel/framework/blob/5.8/src/Illuminate/Foundation/Inspiring.php#L23-L35

> 'When there is no desire, all things are at peace. - Laozi'
> 'Simplicity is the ultimate sophistication. - Leonardo da Vinci',
> 'Simplicity is the essence of happiness. - Cedric Bledsoe',
> 'Smile, breathe, and go slowly. - Thich Nhat Hanh',
> 'Simplicity is an acquired taste. - Katharine Gerould',
> 'Well begun is half done. - Aristotle',
> 'He who is contented is rich. - Laozi',
> 'Very little is needed to make a happy life. - Marcus Antoninus',
> 'It is quality rather than quantity that matters. - Lucius Annaeus Seneca',
> 'Genius is one percent inspiration and ninety-nine percent perspiration. - Thomas Edison',
> 'Computer science is no more about computers than astronomy is about telescopes. - Edsger Dijkstra',
> 'It always seems impossible until it is done. - Nelson Mandela',
> 'Act only according to that maxim whereby you can, at the same time, will that it should become a universal law. - Immanuel Kant'
