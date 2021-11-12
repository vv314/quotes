# Quotes

收集了一些每日一句的接口与网站。

iOS 捷径：[每日一句](https://www.icloud.com/shortcuts/6bb4e30a50584ddb8e791930f1e9f3be)

## 接口集合

> [Postman share link](https://www.getpostman.com/collections/98d52280966545820fe4)

### ONE

-   API：http://v3.wufazhuce.com:8000/api/channel/one/0/0
-   请求方法：`GET`
-   调性：小众，文艺
-   类型：图文

#### 返回值

```json
{
    "res": 0,
    "data": {
        "id": "5829",
        "weather": {},
        "date": "2021-04-07 06:00:00",
        "content_list": [{
            "id": "22156",
            "category": "0",
            "display_category": "4",
            "item_id": "3150",
            "title": "摄影",
            "forward": "大多数人的人生就是这样，你追求的梦想，不一定会在终点给你惊喜，但至少，它会支撑你出发。",
            "img_url": "http://image.wufazhuce.com/Ftv_3DjjyTP-RhBdHLpjObUTvOhl",
            "like_count": 8682,
            "post_date": "2021-04-07 06:00:00",
            "last_update_date": "2021-03-24 17:08:39",
            "author": {},
            "video_url": "",
            "audio_url": "",
            "audio_platform": 2,
            "start_video": "",
            "has_reading": 0,
            "volume": "VOL.3105",
            "pic_info": "Bantersnaps",
            "words_info": "张寒寺《我们这个世界的羊》",
            "subtitle": "",
            "number": 0,
            "serial_id": 0,
            "serial_list": [],
            "movie_story_id": 0,
            "ad_id": 0,
            "ad_type": 0,
            "ad_pvurl": "",
            "ad_linkurl": "",
            "ad_makettime": "",
            "ad_closetime": "",
            "ad_share_cnt": "",
            "ad_pvurl_vendor": "",
            "content_id": "3150",
            "content_type": "0",
            "content_bgcolor": "",
            "share_url": "http://m.wufazhuce.com/one/3150",
            "share_info": {},
            "share_list": {},
            "tag_list": []
        }],
        "menu": {},
        "ad": []
    }
}
```

### 金山词霸

-   API：http://open.iciba.com/dsapi/
-   请求方法：`GET`
-   文档：http://open.iciba.com/?c=wiki
-   调性：励志，鸡汤
-   类型：图文

#### 请求参数

| 属性名 | 默认值   | 必填 | 说明                                              |
| ------ | -------- | ---- | ------------------------------------------------- |
| file   | json     | 否   | 数据格式，默认 json，可选 xml                     |
| date   | 当前日期 | 否   | yyyy-MM-dd，默认当前日期                          |
| type   |          | 否   | date 日期为基准，last 返回前一天，next 返回后一天 |

#### 返回值

注意：响应类型为 `text/html`，需要 JSON 解码

```json
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
            "id": "",
            "name": ""
        }
    ],
    "fenxiang_img": "http://cdn.iciba.com/web/news/longweibo/imag/2019-03-06.jpg"
}
```

### 扇贝单词

-   API：https://apiv3.shanbay.com/weapps/dailyquote/quote
-   请求方法：`GET`
-   调性：励志，鸡汤
-   类型：图文

#### 请求参数

| 属性名 | 默认值   | 必填 | 说明                     |
| ------ | -------- | ---- | ------------------------ |
| date   | 当前日期 | 否   | yyyy-MM-dd，默认当前日期 |

#### 返回值

```json
{
    "id": "bcziue",
    "content": "You can't be paralyzed by fear of failure or you will never push yourself.",
    "author": "Arnold Schwarzenegger",
    "assign_date": "2021-04-07",
    "ad_url": "",
    "share_url": "https://web.shanbay.com/op/quotes/2021-04-07/",
    "share_urls": {},
    "origin_img_urls": [
        "https://media-image1.baydn.com/soup_pub_image/bnznli/c11cffe7ed36219ee44dfee79ceecba4.77390287ed79259b02d8bd7d06f67169.jpeg",
        "https://media-image1.baydn.com/soup_pub_image/bnznli/c11cffe7ed36219ee44dfee79ceecba4.77390287ed79259b02d8bd7d06f67169.jpeg"
    ],
    "share_img_urls": [
        "https://media-image1.baydn.com/soup_pub_image/bnznli/37199a19776d9681c9ccc76d189adc11.6f739349c4584f8b5a050884cd741fae.jpeg",
        "https://media-image1.baydn.com/soup_pub_image/bnznli/37199a19776d9681c9ccc76d189adc11.6f739349c4584f8b5a050884cd741fae.jpeg"
    ],
    "join_num": 43,
    "translation": "你绝不能为失败的恐惧所吓倒，否则你将永远不会前进。",
    "poster_img_urls": [
        "https://media-image1.baydn.com/dailyquote/url-79491420f4846dd98cf5b61d5f5381fee98a7b3159349a07334d78acb4d90343.jpg?x-oss-process=image/quality,Q_80/format,webp",
        "https://media-image1.baydn.com/dailyquote/url-79491420f4846dd98cf5b61d5f5381fee98a7b3159349a07334d78acb4d90343.jpg?x-oss-process=image/quality,Q_80/format,webp"
    ],
    "track_object": {},
    "daily_audio_urls": ""
}
```

### 一言

-   API：https://v1.hitokoto.cn/
-   请求方法：`GET`
-   官网：https://hitokoto.cn/
-   文档：https://hitokoto.cn/api
-   调性：二次元，网络，中二
-   类型：文字

#### 请求参数

| 属性名   | 默认值   | 必填 | 说明                                                          |
| -------- | -------- | ---- | ------------------------------------------------------------- |
| c        | 随机     | 否   | a: 动画, b: 漫画, c: 游戏, d: 小说, e: 原创, f: 网络, g: 其他 |
| encode   | json     | 否   | 可选值：text, json, js，当指定 js 时返回 jsonp                |
| charset  | utf-8    | 否   | 可选值：utf-8, gbk                                            |
| callback | hitokoto | 否   | jsonp 函数名，与 encode: js 配合使用                          |

#### 返回值

```json
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

-   API：https://v2.jinrishici.com/one.json
-   请求方法：`GET`
-   官网：https://www.jinrishici.com/
-   文档：https://www.jinrishici.com/doc/
-   调性：诗词，古风
-   类型：文字

#### 返回值

```json
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
            "translate": ""
        },
        "matchTags": ["白天", "桃花"],
        "recommendedReason": "",
        "cacheAt": "2019-03-06T16:46:48.003082"
    },
    "token": "1L+kOwPjxE0+1mtlehoED8XuDj11JncZ",
    "ipAddress": "61.135.152.135",
    "warning": ""
}
```

### Storm

-   API：http://quotes.stormconsultancy.co.uk/random.json
-   请求方法：`GET`
-   官网：http://quotes.stormconsultancy.co.uk/
-   文档：http://quotes.stormconsultancy.co.uk/api
-   调性：计算机，编程领域
-   类型：文字

#### 返回值

```json
{
    "author": "E. W. Dijkstra",
    "id": 14,
    "quote": "If debugging is the process of removing software bugs, then programming must be the process of putting them in.",
    "permalink": "http://quotes.stormconsultancy.co.uk/quotes/14"
}
```

## 编程领域

### 网站

-   http://www.defprogramming.com
-   https://skolakoda.org/programming-quotes/#/
-   http://quotes.stormconsultancy.co.uk/
-   https://en.wikiquote.org/w/api.php
-   https://www.goodreads.com/quotes/tag/programming
-   https://www.brainyquote.com/topics/programming

### Github

-   API：https://api.github.com/zen
-   请求方法：`GET`
-   调性：启发，哲学
-   类型：文字

#### 返回值

```
Keep it logically awesome.
```

全部数据：https://gist.github.com/sorrycc/7214622

```
- "It's not fully shipped until it's fast."
- "Practicality beats purity."
- "Avoid administrative distraction."
- "Mind your words, they are important."
- "Non-blocking is better than blocking."
- "Design for failure."
- "Half measures are as bad as nothing at all."
- "Favor focus over features."
- "Approachable is better than simple."
- "Encourage flow."
- "Anything added dilutes everything else."
- "Speak like a human."
- "Responsive is better than fast."
- "Keep it logically awesome."
```

### laravel inspire

https://github.com/laravel/framework/blob/5.8/src/Illuminate/Foundation/Inspiring.php#L23-L35

```
- 'When there is no desire, all things are at peace. - Laozi'
- 'Simplicity is the ultimate sophistication. - Leonardo da Vinci'
- 'Simplicity is the essence of happiness. - Cedric Bledsoe'
- 'Smile, breathe, and go slowly. - Thich Nhat Hanh'
- 'Simplicity is an acquired taste. - Katharine Gerould'
- 'Well begun is half done. - Aristotle'
- 'He who is contented is rich. - Laozi'
- 'Very little is needed to make a happy life. - Marcus Antoninus'
- 'It is quality rather than quantity that matters. - Lucius Annaeus Seneca'
- 'Genius is one percent inspiration and ninety-nine percent perspiration. - Thomas Edison'
- 'Computer science is no more about computers than astronomy is about telescopes. - Edsger Dijkstra'
- 'It always seems impossible until it is done. - Nelson Mandela'
- 'Act only according to that maxim whereby you can, at the same time, will that it should become a universal law. - Immanuel Kant'
```
