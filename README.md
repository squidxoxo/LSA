# 猜歌遊戲 README

[![hackmd-github-sync-badge](https://hackmd.io/ktRec9XuQniTA3w9MsG5xw/badge)](https://hackmd.io/ktRec9XuQniTA3w9MsG5xw)


## 事前準備
1. [Download Python](https://www.python.org/downloads/)
2. 確認你的`python`及`pip`有成功安裝
```shell=
python --version
# 版本須為3.x.x
pip --version
# 版本須為3.x.x
```
3. 安裝
```shell=
pip install telepot
pip install python3-telepot
pip install re2
pip install vlc
pip install python3-vlc
pip install pafy
pip install urllib
pip install python3-urllib
```

## 遊戲玩法
1. 將 telegram bot 加入群組
2. 成員選擇`/join`加入遊戲
3. 選擇`/start`開始遊戲並顯示遊戲規則
4. 輸入 `/music` + **歌手名** 並開始遊戲
5. 遊戲共有 5 關，每關 3 題，並依據關卡難度提高得分
6. 若該題無人回答正確，則可使用提示`/promt`，**但使用提示會降低得分**
7. 遊戲全部結束，列出得分**前三高**的分數

|關卡| 1| 2| 3| 4|5|
| -------- | -------- | -------- |--------|---------|-------|
| 關卡的秒數 | 60 | 30 |   20 |  10 | 5|
| 關卡的計分方式  | 5 | 10 |  15|   20|  25|
| 使用提示後的得分 |  3 |  6 |  9| 12 |15| 

## 遊戲控制
- `/join` 加入遊戲
- `/start` 開始遊戲
- `/music 歌手` 設定遊戲範圍
- `/replay` 重新播放題目
- `/exit` 離開遊戲
- `/pass` 跳過此題
- `/prompt` 顯示提示
- `/rank` 列出排名前三高