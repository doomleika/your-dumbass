# Dumbass

這位老兄原本指控用 process monitor 看的

![這位老兄原本指控用 process monitor 看的](https://github.com/doomleika/your-dumbass/blob/master/img/the-idiot-zero.jpeg)

這邊有一位電腦高手認為 electron 不會看憑證

![u wot?](https://github.com/doomleika/your-dumbass/blob/master/img/u-wot1.png)

![u wot2?](https://github.com/doomleika/your-dumbass/blob/master/img/u-wot2.png)

## 呵

示範給你看，code是直接從[官方 electron 範例](https://github.com/electron/electron-quick-start) clone 過來的

打開 [process monitor](https://docs.microsoft.com/en-us/sysinternals/downloads/procmon)

設定filter

* `Process Name` __is__ `electron.exe`
* `path` __containers__ `Certificates`

![filter](https://github.com/doomleika/your-dumbass/blob/master/img/filters.png)

```bash
npm install
npm start
```

體會一下自己計算機概論是怎麼pass的

![electron](https://github.com/doomleika/your-dumbass/blob/master/img/electrion-cert.png)

Epic Game Launcher是長這樣

![egl](https://github.com/doomleika/your-dumbass/blob/master/img/egl.png)


弱弱問一下問差別在哪?

不要跟我說 `mainWindow.loadFile('index.html')` 換成 `mainWindow.loadURL('https://github.com')` 不算數，難道EGL到它們的Server不用 `HTTPS` 連線敢情是用小叮噹任意門來著?

## 順便讓你看一下別的 launcher 會怎麼樣

### steam

![steam](https://github.com/doomleika/your-dumbass/blob/master/img/steam.png)


### Uplay

![uplay](https://github.com/doomleika/your-dumbass/blob/master/img/uplay.png)


只要是要HTTPS連線，一定會用到憑證。

## 送你一句

[![shut up](https://github.com/doomleika/your-dumbass/blob/master/img/have-a-nice-big-cup-of-shut-the-fuck-up.png)](https://www.reddit.com/r/PhoenixPoint/comments/b0rxdq/epic_game_store_spyware_tracking_and_you/eikhtip?utm_source=share&utm_medium=web2x)
