ck101-downloader 卡提諾圖片下載器
======================
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/kkdai/ck101-downloader/master/LICENSE) [![Build Status](https://travis-ci.org/kkdai/ck101-downloader.svg)](https://travis-ci.org/kkdai/ck101-downloader)


`ck101-downloader`是一個小的console app，可以瀏覽[卡提諾](http://ck101.com)的[熱議美女](http://ck101.com/forum-3285-1.html)版面．

這個程式主要是透過[Photomgr](http://github.com/kkdai/photomgr)來讀取資料，該模組有支援更多的網站．

他可以透過console mode去瀏覽主要標題，並且指定哪些文章可以下載裡面的所有圖片到你的電腦中．


安裝
--------------

    go get -u -x github.com/kkdai/ck101-downloader

使用
---------------------

    ck101-downloader  

所有的圖片會安裝到 `USERS/Pictures/iloveptt` 並且會依照文章的標題分開不同的資料夾．

如果你是Windows使用者，他會自動存取到你的使用者資料夾的圖片之中．



選項
---------------

- `-w` 選定下載同步的執行序列個數，預設是10


交互指令
---------------

目前支援所有的指令如下:

- `n`: 顯示下一頁的資料.
- `p`: 顯示前一夜的資料.
- `o`: 打開目前的資料夾.
- `d` number: 下載該文章的所有圖片到你的電腦中.
- `quit`: 離開目前程式.

範例
---------------

簡單的範例透過設定同步10個下載序列來瀏覽.

        //Run app.
        ck101-downloader -w=10
        
        0:[1★][正妹] 勇敢的女孩
        1:[0★](本文已被刪除) [ao3sm345]
        2:[0★](本文已被刪除) [chuhengyi820]
        3:[0★](本文已被刪除) [titan3417]
        4:[8★][公告] 不願上表特 ＆ 優文推薦 ＆ 檢舉建議專區
        ......
        >ptt>

        //Download index [5].
        d 5
        
        //quit application
        quit
     


Snapshot
---------------

![image](snapshot/1.png)



Inspired
---------------

This project inspired from [https://github.com/tzangms/iloveck101](https://github.com/tzangms/iloveck101). And I refer those implements as follow:

- Photo download and CLI: [https://github.com/lazywei/iloveck101](https://github.com/lazywei/iloveck101)


Contribute
---------------

Please open up an issue on GitHub before you put a lot efforts on pull request.
The code submitting to PR must be filtered with `gofmt`


廣告
---------------

如果你喜歡這個App，請考慮以下方式贊助我

- 請花30塊買小弟的[粉絲相簿](https://itunes.apple.com/tw/app/fen-si-xiang-bu/id839324997?l=zh&mt=8) App．
- 按下一個"github Star"

感謝...

想要iOS的版本？
---------------

這裡有簡單的版本可以下載並且自己安裝 [PhotoViewer](https://github.com/kkdai/PhotoViewer)

Project52
---------------

It is one of my [project 52](https://github.com/kkdai/project52).


License
---------------

This package is licensed under MIT license. See LICENSE for details.
