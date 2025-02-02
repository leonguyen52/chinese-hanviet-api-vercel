## Overview
![Alt text](/../main/screenshots/ScreenShot%202025-02-03%20at%2005.29.38.jpg?raw=true "Homepage")
An API built using [json-server](https://github.com/typicode/json-server) that allows you to look up Chinese and Han Viet cognates.\n
* This original idea is started by [ryanphung](https://github.com/ryanphung) and I updated it to match my own requirements with new database + add new function for personal use.

It will be divided into 2 type "tughep" (compoud words) and "tudon" (single word) while looking up dictionary.
* /tughep 23940x words
* /tudon 11411x words

## Demo

* https://cndict.lukobi.com/tughep?hanviet=nhân%20vi
* https://cndict.lukobi.com/tughep?meaning=còn%20có
* https://cndict.lukobi.com/tughep?pinyin=zhèxiē
* https://cndict.lukobi.com/tudon?word_like=可
* https://cndict.lukobi.com/tudon?hanviet=nhất

## Sample Response

Sample Response - Từ Ghép:
```
[{
    "chinese word ranking": 0,
    "frequency": 2837.94,
    "word": "我们",
    "traditional": "我們",
    "pinyin": "wǒmen",
    "hanviet": "ngã môn",
    "meaning": "chúng ta/chúng tôi/chúng tao/chúng tớ"
}]
```

Sample Response - Từ Đơn:
```
[{
    "word": "人",
    "hanviet": "nhân",
    "pronunciation": "r: uốn cong lưới đầu lưỡi đặt ở ngạc cứng hàm răng trên: đọc là ân"
}]
```

## Search Web App
I also created a simple HTML Web App to query based on this API. 
You can fill in multiple Chinese words and it will break down to query data and return result
![Alt text](/../main/screenshots/ScreenShot%202025-02-03%20at%2005.30.39.jpg?raw=true "Search App")
