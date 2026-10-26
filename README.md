# Steam 创意工坊批量订阅提取器

这是一个运行在浏览器控制台的 JavaScript 脚本，用于一键提取你在 Steam 创意工坊中订阅的所有 MOD/物品链接，并自动生成批量订阅脚本。

## ⚠️ 免责声明

**事先说明，此脚本仅供学习交流使用，切勿用于非法用途。请支持正版游戏，尊重每一位游戏开发者的劳动成果。** 使用本脚本所产生的一切后果由使用者自行承担。

## ✨ 功能特点

- 无需安装任何环境，直接在浏览器控制台运行。
- 自动解析当前页面的 APPID。
- 后台静默抓取，无需手动翻页。

## 适用平台
- Windows 7 以上   (Windows 10 1809之前版本SteamCMD可能不稳定)
- Linux   glibc >= 2.12
- macOS   OS X 10.11 (El Capitan) 	仅限 Intel Mac,且需确认游戏服务端是否支持

## 图形化替代
可以使用由**lu-cent**制作的[WorkshopDL-PS](https://github.com/lu-cent/WorkshopDL-PS)
注意:只支持windows系统，需要**PowerShell 5.1+**

## 🛠️ 使用方法

1. 登录 [Steam 网页版](https://steamcommunity.com/)。
2. 进入你的特定游戏订阅页面（例如：`https://steamcommunity.com/profiles/xxx/myworkshopfiles?appid=294100&browsefilter=mysubscriptions&p=1&numperpage=30`）。
3. 按下 `F12` 打开浏览器开发者工具，点击 `Console`（控制台）标签。
4. 将 `main.js` 中的代码粘贴到控制台中，并按回车运行。
5. 脚本运行完毕后，浏览器会自动下载一个名为 `steamcmd_app_XXXXX.txt` 的文件。
6. 将下载的 `.txt` 里面的 `JS` 订阅脚本复制，发给其他人。
7. 其他人想要订阅只需要打开一个任意创意工坊物品（[比如](https://steamcommunity.com/sharedfiles/filedetails/?id=1623423360)）然后在控制台运行订阅脚本。

## 如果是 `id` 列表

1. 如果已经有 `id` 列表了的话，可以先随便订阅几个 `mod`，然后运行一下 `main.js` 获得示例订阅脚本（下载的 `.txt`）
2. 将示例订阅脚本里的数字`{ id: '某个数字', appId: '某个数字' }, ...`改成自己想要的就行。
3. 可以发给`AI`来改，非常简单，后续还是需要打开一个任意创意工坊物品，然后在控制台运行订阅脚本。

## 相关项目
[WorkshopDL-PS](https://github.com/lu-cent/WorkshopDL-PS)
