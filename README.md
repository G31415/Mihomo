# Mihomo 图标库

mihomo / Clash.Meta 配置用的图标集合，共 **347 个 PNG**，用于 `proxy-groups` 的 `icon` 字段，也可用于策略组、规则的视觉区分。

所有图标位于 [`icon/`](./icon) 目录。

## 引用方式

下面的链接已按本仓库的实际地址填好，把 `<图标名>` 换成清单里的名字，直接复制即可使用。

### jsDelivr CDN（推荐）

```
https://cdn.jsdelivr.net/gh/G31415/Mihomo@main/icon/<图标名>.png
```

境外 CDN，速度快，适合大多数客户端。

### GitHub Raw

```
https://raw.githubusercontent.com/G31415/Mihomo/main/icon/<图标名>.png
```

## 在 mihomo 中使用

```yaml
proxy-groups:
  - name: 🍎 Apple
    type: select
    icon: https://cdn.jsdelivr.net/gh/G31415/Mihomo@main/icon/Apple.png
    proxies:
      - DIRECT
      - 自动选择

  - name: 📺 流媒体
    type: select
    icon: https://cdn.jsdelivr.net/gh/G31415/Mihomo@main/icon/Streaming.png
    proxies:
      - 香港
      - 新加坡
      - 日本

  - name: 🤖 AI
    type: select
    icon: https://cdn.jsdelivr.net/gh/G31415/Mihomo@main/icon/ChatGPT.png
    proxies:
      - 美国
      - 日本
```

> 提示：`icon` 只在支持的客户端（Clash Verge Rev、Mihomo Party、FlClash 等）中显示，Clash for Windows 不显示。

## 注意事项

**特殊字符**：以下图标名含有 `+`、`&`、`!` 等字符。它们本身是合法的 URL 路径字符，绝大多数客户端可直接使用；若遇到个别客户端解析异常，做百分号转义即可：

| 图标名 | 转义写法 |
| --- | --- |
| `Apple_Fitness+` | `Apple_Fitness%2B` |
| `Apple_Fitness+_Letter` | `Apple_Fitness%2B_Letter` |
| `discovery+` | `discovery%2B` |
| `Disney+` | `Disney%2B` |
| `ESPN+` | `ESPN%2B` |
| `Star+` | `Star%2B` |
| `iQIYI&bilibili` | `iQIYI%26bilibili` |
| `Streaming!CN` | `Streaming%21CN` |

**CDN 缓存**：jsDelivr 对 `@main` 分支的缓存约 12 小时。更新图标后想立即生效，可访问下面的地址手动刷新：

```
https://purge.jsdelivr.net/gh/G31415/Mihomo@main/icon/Apple.png
```

固定版本可以用 commit hash 或 tag 代替 `@main`，例如 `@v1`。

**本地使用**：如果客户端支持从文件系统读取图标，直接用 `icon/Apple.png` 这类相对路径即可，无需联网。

## 图标清单

<details>
<summary>点击展开全部 347 个图标名</summary>

```
5iTV
AbemaTV
AdBlack
Advertising
AdWhite
AfreecaTV
Africa_Map
AGA
AI
AIA
Airport
Alibaba
All4
Amazon
Amazon_1
America_Map
AmyTelecom
AmyTelecom_1
Apeach
App_Store
Apple
Apple_1
Apple_2
Apple_Fitness
Apple_Fitness+
Apple_Fitness+_Letter
Apple_Music
Apple_News
Apple_TV
Apple_TV_Plus
Apple_Update
AR
Area
Argentina
Asia_Map
AU
Australia
Auto
Available
Available_1
Azure
Back
Bahamut
Bamboo
BBC_iPlayer
BBC_iPlayer_1
BBC_iPlayer_2
BGP
bilibili
bilibili_1
bilibili_2
bilibili_3
bilibili_4
Blackhole
Blinkload
Blinkload_1
Bookpedia
BosLife
BosLife_1
Bot
BR
Brazil
Brown
Bypass
CA
Canada
Cat
Catnet
CC
Cellular
ChatGPT
China
China_Map
Cloudflare
Clubhouse
Clubhouse_1
Clubhouse_2
CN
Copilot
CreamData
Cryptocurrency
Cryptocurrency_1
Cryptocurrency_2
Cryptocurrency_3
Cydia
Daily
DAZN
DAZN_1
DAZN_2
DE
deezer
deezer_1
deezer_2
Dinosaur
Direct
Discord
discovery+
Disney
Disney+
Disney+_1
Disney+_2
Domestic
DomesticMedia
Download
Drill
EG
Egypt
Emby
encoreTVB
Epic_Games
ESPN+
ESPN+_1
ESPN+_2
EU
Europe_Map
European_Union
Facebook
FI
Filter
Final
Final_1
Find_My
Finland
Flamingo
ForeignMedia
FOX
FR
France
friDay
Fries
Frog
fuboTV
Game
Germany
GIA
GitHub
GitHub_Letter
Global
Gmail
Google
Google_Drive
Google_Opinion_Rewards
Google_Search
HBO
HBO_1
HBO_2
HBO_GO
HBO_GO_1
HBO_GO_2
HBO_Max
HC
Heart
Hijacking
HK
HKMTMedia
Hong_Kong
Hulu
Hulu_1
iCloud
IEPL
IN
India
Infuse
Infuse_7
Ingress
Instagram
IPLC
iQIYI
iQIYI&bilibili
iQIYI_1
ITV
ITV_1
ITV_2
Japan
JOOX
JP
Kakao
KKBOX
KKTV
Korea
KR
LA
LA_Map
Lab
Lambda
League_of_Legends
Line
LineTV
LinkCube
Linkedin
LiTV
Lock
LOL
Loop
Luffy
Macao
Magic
Mail
Malaysia
Media
Mickey
Microsoft
MO
Mouse
Music_Enhance
MY
My5
myTV_SUPER
Naiko
NBA
NBC
Netease_Music
Netease_Music_Unlock
Netflix
Netflix_Letter
Nfcloud
niconico
niconico_1
niconico_2
Ninja
Nintendo
Notion
nowe
Null_Nation
Oceania_Map
OneDrive
Ox
Panda
Pandora
Paramount
PayPal
PBS
Peacock
Peacock_1
Peacock_2
PH
Philippines
Pig
Pirate_Nation
PlayStation
PlayStation_1
Pornhub
Pornhub_1
Pornhub_2
PostBox
PostBox_1
Prime_Video
Prime_Video_1
Prime_Video_2
Proxy
Puzzle
QQ
Quantumult_X
Qure
Rainbow
Rainbow_1
Reject
Renzhe
Ring
Rocket
Round_Robin
Round_Robin_1
RU
Russia
Ryan
Scholar
Server
SG
Singapore
Siri
Sling_TV
Spark
Speedtest
Spotify
SSID
SSID_1
SSL
ssLinks
Stack
Star
Star_1
Star_2
Star+
STARZ
Static
Static_1
Steam
Streaming
Streaming!CN
StreamingCN
StreamingSE
TAG
Taiwan
Taobao
Telegram
Telegram_X
TestFlight
TestFlight_1
TestFlight_2
TH
Thailand
TIDAL
TIDAL_1
TIDAL_2
TikTok
TikTok_1
TikTok_2
TR
Tubi
Turkey
TVB
TW
Twitch
Twitter
UA
UK
Ukraine
ULB
ULB_1
UN
United_Kingdom
United_Nations
United_States
United_States_Map
Unlock
US
Vimeo
VIP
Viu
ViuTV
Want_Want
Want_Want_1
WeChat
Weibo
WeTV
WeTV_Letter
WiFi
Windows
Windows_11
World_Map
X
Xbox
Yahoo
Yahoo_1
YouTube
YouTube_Letter
YouTube_Music
```

</details>

## 常用图标速查

按用途挑几个常用的，省得翻清单：

| 用途 | 图标名 |
| --- | --- |
| 自动选择 / 故障转移 | `Auto`、`Available`、`Round_Robin`、`Global` |
| 直连 / 拒绝 | `Direct`、`Reject`、`Bypass`、`AdBlack`、`Advertising` |
| 兜底 / 漏网之鱼 | `Final`、`Blackhole`、`Filter` |
| AI | `AI`、`ChatGPT`、`Copilot`、`Lambda`、`Scholar` |
| 流媒体 | `Streaming`、`Netflix`、`Disney+`、`YouTube`、`Spotify` |
| 地区 | `HK`、`TW`、`JP`、`SG`、`US`、`UK`、`KR`、`DE`、`FR` |
| 机场 / 线路 | `Airport`、`IEPL`、`IPLC`、`BGP`、`GIA`、`Lambda` |
| 下载 / 测速 | `Download`、`Speedtest`、`GitHub`、`Steam` |

---

图标版权归各自所有者，本仓库仅作整理收集。
