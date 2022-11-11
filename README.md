<div align="center">
  <h1 align="center">TweetFeed</h1>

  <p align="center">
    Feeds of IOCs posted on Twitter
    <br />
    <br />
    <strong>Web version at <a href="https://tweetfeed.live/">TweetFeed.live</a></strong> / <strong>Code at <a href="https://github.com/0xDanielLopez/TweetFeed_code">TweetFeed (code)</a></strong>
  </p>

  ![TweetFeed.live](https://raw.githubusercontent.com/TweetFeed/TweetFeed.github.io/main/img/TweetFeed_live.PNG)
</div>

## Content

- [Data collected](#data-collected)
- [Some statistics](#some-statistics)
- [How it works](#how-it-works)
- [Hunting IOCs via Microsoft Defender](#hunting-IOCs-via-Microsoft-Defender)
- [Author](#author)
- [Disclaimer](#disclaimer)

## Give a Star! :star:
If you like the project, please consider giving it a star!

## Data collected

<table>
    <thead>
        <tr>
		<th colspan=4><b>Feeds</b></th>
        </tr>
    </thead>
    <tbody>
	<tr>
		<th colspan=4>2022-11-11 06:35:44 (UTC)</th>
	</tr>
    <tr>
            <th>Today</th>
            <th>Last 7 days</th>
            <th>Last 30 days</th>
            <th>Last 365 days</th>
    </tr>
    <tr>
            <td>:clipboard: <a href="https://github.com/0xDanielLopez/TweetFeed/blob/master/today.csv">Today</a> (<a href="https://raw.githubusercontent.com/0xDanielLopez/TweetFeed/master/today.csv">raw</a>)</td>
            <td>:clipboard: <a href="https://github.com/0xDanielLopez/TweetFeed/blob/master/week.csv">Week</a> (<a href="https://raw.githubusercontent.com/0xDanielLopez/TweetFeed/master/week.csv">raw</a>)</td>
            <td>:clipboard: <a href="https://github.com/0xDanielLopez/TweetFeed/blob/master/month.csv">Month</a> (<a href="https://raw.githubusercontent.com/0xDanielLopez/TweetFeed/master/month.csv">raw</a>)</td>
            <td>:clipboard: <a href="https://github.com/0xDanielLopez/TweetFeed/blob/master/year.csv">Year</a> (<a href="https://raw.githubusercontent.com/0xDanielLopez/TweetFeed/master/year.csv">raw</a>)</td>
     </tr>
    </tbody>
</table>

#### Output example 

<table>
	<thead>
		<tr>
			<th><sub>Date (UTC)</sub></th>
			<th><sub>SourceUser</sub></th>
			<th><sub>Type</sub></th>
			<th><sub>Value</sub></th>
			<th><sub>Tags</sub></th>
			<th><sub>Tweet</sub></th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td><sub>2021-08-14 02:26:32</sub></td>
			<td><sub>phishunt_io</sub></td>
			<td><sub>url</sub></td>
			<td><sub>https://netflix.us2.cards/</sub></td>
			<td><sub>#phishing #scam</sub></td>
			<td><sub>https://twitter.com/phishunt_io/status/1426369619422502917</sub></td>
		</tr>
		<tr>
			<td><sub>2021-08-17 12:15:00</sub></td>
			<td><sub>TheDFIRReport</sub></td>
			<td><sub>ip</sub></td>
			<td><sub>185.56.76.94</sub></td>
			<td><sub>#Trickbot</sub></td>
			<td><sub>https://twitter.com/TheDFIRReport/status/1427604874053578756</sub></td>
		</tr>
	</tbody>
</table>

## Some statistics

#### IOCs

| IOC | Today | Week | Month | Year |
| :--- | :---: | :---: | :---: | :---: |
| **:link: URLs** | 212 | 4547 | 17582 | 153942 |
| **:globe_with_meridians: Domains** | 102 | 382 | 2915 | 30001 |
| **:triangular_flag_on_post: IPs** | 44 | 670 | 3359 | 56955 |
| **:1234: SHA256** | 0 | 79 | 394 | 20437 |
| **:1234: MD5** | 20 | 255 | 2004 | 5428 |

#### Tags

| Tag | Today | Week | Month | Year |
| :--- | :---: | :---: | :---: | :---: |
| **#phishing** | 251 | 2588 | 13623 | 184133 |
| **#scam** | 125 | 672 | 4296 | 34880 |
| **#malware** | 108 | 2698 | 9661 | 26849 |
| **#maldoc** | 0 | 2 | 3 | 219 |
| **#ransomware** | 10 | 51 | 558 | 1244 |
| **#banker** | 0 | 0 | 6 | 33 |
| **#AgentTesla** | 0 | 1 | 32 | 2753 |
| **#Alienbot** | 0 | 0 | 0 | 11 |
| **#BazarLoader** | 0 | 0 | 0 | 160 |
| **#CobaltStrike** | 6 | 281 | 1226 | 19765 |
| **#Dridex** | 0 | 0 | 0 | 584 |
| **#Emotet** | 1 | 73 | 142 | 1756 |
| **#FluBot** | 0 | 0 | 1 | 11 |
| **#Follina** | 0 | 0 | 3 | 152 |
| **#Formbook** | 0 | 0 | 21 | 2470 |
| **#GootLoader** | 0 | 10 | 20 | 721 |
| **#GuLoader** | 0 | 0 | 7 | 220 |
| **#Hancitor** | 0 | 0 | 0 | 45 |
| **#IcedID** | 1 | 38 | 74 | 513 |
| **#Lazarus** | 3 | 5 | 13 | 163 |
| **#Lokibot** | 0 | 2 | 16 | 951 |
| **#log4j** | 0 | 0 | 0 | 247 |
| **#Log4shell** | 0 | 0 | 0 | 231 |
| **#ProxyNotShell** | 0 | 0 | 2 | 2 |
| **#ProxyShell** | 0 | 0 | 0 | 15 |
| **#Qakbot** | 0 | 0 | 11 | 300 |
| **#Raccoon** | 0 | 6 | 17 | 675 |
| **#RedLine** | 0 | 4 | 55 | 2721 |
| **#Remcos** | 0 | 2 | 21 | 592 |
| **#Spring4Shell** | 0 | 0 | 0 | 26 |
| **#Trickbot** | 0 | 0 | 0 | 43 |
| **#Ursnif** | 0 | 2 | 6 | 356 |

#### Top reporters (today)

| Number | User | IOCs | 
| :--- | :---: | :---: | 
| **#1** | [ecarlesi](https://twitter.com/ecarlesi) | 166 |
| **#2** | [pingineer_jp](https://twitter.com/pingineer_jp) | 109 |
| **#3** | [romonlyht](https://twitter.com/romonlyht) | 28 |
| **#4** | [RedPacketSec](https://twitter.com/RedPacketSec) | 19 |
| **#5** | [AP_Zenmashi](https://twitter.com/AP_Zenmashi) | 14 |
| **#6** | [KesaGataMe0](https://twitter.com/KesaGataMe0) | 9 |
| **#7** | [drb_ra](https://twitter.com/drb_ra) | 6 |
| **#8** | [RdpSnitch](https://twitter.com/RdpSnitch) | 4 |
| **#9** | [quicksandphish](https://twitter.com/quicksandphish) | 4 |
| **#10** | [Cryptolaemus1](https://twitter.com/Cryptolaemus1) | 3 |

## How it works?
Search tweets that contain certain tags **or** that are posted by certain *infosec* people.

### Tags being searched
##### *(not case sensitive)*
```
- #phishing
- #scam
- #malware
- #maldoc
- #ransomware
- #banker
- #AgentTesla
- #Alienbot
- #BazarLoader
- #CobaltStrike
- #Dridex
- #Emotet
- #FluBot
- #Follina
- #Formbook
- #GootLoader
- #GuLoader
- #Hancitor
- #IcedID
- #Lazarus
- #Lokibot
- #log4j
- #Log4shell
- #ProxyNotShell
- #ProxyShell
- #Qakbot
- #Raccoon
- #RedLine
- #Remcos
- #Spring4Shell
- #Trickbot
- #Ursnif
```


### Also search Tweets posted by
##### *(these are trusted folks that sometimes don't use tags)*
<big><pre>
[**TweetFeed list**](https://twitter.com/i/lists/1423693426437001224)
</pre></big>


### IOCs being collected
```
- URL
- Domain
- IP address
- SHA256 hash
- MD5 hash
```

## Hunting IOCs via Microsoft Defender

**1. Search `SHA256` hashes with `yearly` tweets feed**
```kusto
let MaxAge = ago(30d);
let SHA256_whitelist = pack_array(
'XXX' // Some SHA256 hash you want to whitelist.
);
let TweetFeed = materialize (
    (externaldata(report:string)
    [@"https://raw.githubusercontent.com/0xDanielLopez/TweetFeed/master/year.csv"]
    with (format = "txt"))
    | extend report = parse_csv(report)
    | extend Type = tostring(report[2])
    | where Type == 'sha256'
    | extend SHA256 = tostring(report[3])
    | where SHA256 !in(SHA256_whitelist)
    | extend Tag = tostring(report[4])
    | extend Tweet = tostring(report[5])
    | project SHA256, Tag, Tweet 
);
union (
    TweetFeed
    | join (
        DeviceProcessEvents
        | where Timestamp > MaxAge
    ) on SHA256
), (
    TweetFeed
    | join (
        DeviceFileEvents
        | where Timestamp > MaxAge
    ) on SHA256
), ( 
    TweetFeed
    | join (
        DeviceImageLoadEvents
        | where Timestamp > MaxAge
    ) on SHA256
) | project Timestamp, DeviceName, FileName, FolderPath, SHA256, Tag, Tweet
```

<br>

**2. Search `IP addresses` with `monthly` tweets feed**
```kusto
let MaxAge = ago(30d);
let IPaddress_whitelist = pack_array(
'XXX' // Some IP address you want to whitelist.
);
let TweetFeed = materialize (
    (externaldata(report:string)
    [@"https://raw.githubusercontent.com/0xDanielLopez/TweetFeed/master/month.csv"]
    with (format = "txt"))
    | extend report = parse_csv(report)
    | extend Type = tostring(report[2])
    | where Type == 'ip'
    | extend RemoteIP = tostring(report[3])
    | where RemoteIP !in(IPaddress_whitelist)
    | where not(ipv4_is_private(RemoteIP))
    | extend Tag = tostring(report[4])
    | extend Tweet = tostring(report[5])
    | project RemoteIP, Tag, Tweet 
);
union (
TweetFeed
    | join (
        DeviceNetworkEvents
    | where Timestamp > MaxAge
    ) on RemoteIP
) | project Timestamp, DeviceName, RemoteIP, Tag, Tweet
```

<br>

**3. Search `urls` and `domains` with `weekly` tweets feed**
```kusto
let MaxAge = ago(30d);
let domain_whitelist = pack_array(
'XXX' // Some URL/Domain you want to whitelist.
);
let TweetFeed = materialize (
    (externaldata(report:string)
    [@"https://raw.githubusercontent.com/0xDanielLopez/TweetFeed/master/week.csv"]
    with (format = "txt"))
    | extend report = parse_csv(report)
    | extend Type = tostring(report[2])
    | where Type in('url','domain')
    | extend RemoteUrl = tostring(report[3])
    | where RemoteUrl !in(domain_whitelist)
    | extend Tag = tostring(report[4])
    | extend Tweet = tostring(report[5])
    | project RemoteUrl, Tag, Tweet 
);
union (
TweetFeed
    | join (
        DeviceNetworkEvents
    | where Timestamp > MaxAge
    ) on RemoteUrl
) | project Timestamp, DeviceName, RemoteUrl, Tag, Tweet
```

## Author
* [**Daniel López**](https://twitter.com/0xDanielLopez)

<!--- ![Twitter](https://img.icons8.com/officexs/16/000000/twitter.png) --->

## Disclaimer

Please note that all the data is collected from Twitter and sorted/served here as it is on best effort.

I have tried to tune as much as possible the searches trying to collect only valuable info. However please consider making your own analysis before taking any action related to these IOCs.

Anyway feel free to reach me out regarding any False Positive or to provide any kind of feedback.

<hr>

By the Community for the Community
