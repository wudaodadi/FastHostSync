# SteamHostSync
第一次用go写的项目，写的比较烂，欢迎大佬指出错误。

## 1. 实现
对Hosts进行一个新的更  
解决Steam、github访问问题

## 2. 使用方法
## 自动方法(使用工具)
推荐使用Hosts管理工具[SwitchHosts](https://github.com/oldj/SwitchHosts) 
[SwitchHosts备用下载源](https://nas.iaimi.info/s/nT5pb8jMQp32QwB)
### 开机自启动SwitchHosts
win + R 后执行 `shell:startup`    
![](/img/1.png)  
将快捷方式复制进去即可  
![](/img/2.png)  
### 配置SwitchHosts实现自动更新  
可选的URL有:
如果访问不到GitHub可以尝试将`github.com`替换为`hub.fastgit.xyz`(国内镜像)
1. ALL: `https://raw.githubusercontent.com/Clov614/SteamHostSync/main/Hosts`  
2. Steam: `https://raw.githubusercontent.com/Clov614/SteamHostSync/main/Hosts_steam`  
3. github: `https://raw.githubusercontent.com/Clov614/SteamHostSync/main/Hosts_github`    
`镜像地址:`
4. All: `https://raw.sevencdn.com/Clov614/SteamHostSync/main/Hosts`  
5. Steam: `https://raw.sevencdn.com/Clov614/SteamHostSync/main/Hosts_steam`  
6. github: `https://raw.sevencdn.com/Clov614/SteamHostSync/main/Hosts_github`  

![](/img/3.png)

## 手动方式
#### 1. hosts 文件在每个系统的位置不一，详情如下:
- Windows 系统：`C:\Windows\System32\drivers\etc\hosts`
- Linux 系统：`/etc/hosts`
- Mac（苹果电脑）系统：`/etc/hosts`

#### 2. 修改方法
复制下面的内容至hosts尾部(追加在文本末尾)

```
#github Start
140.82.114.26			alive.github.com
185.199.109.154			docs.github.com
140.82.114.25			live.github.com
140.82.116.14			uploads.github.com
185.199.108.153			training.github.com
185.199.111.133			objects.githubusercontent.com
185.199.110.153			metamask.github.io
185.199.111.153			pages.github.com
13.107.42.16			pipelines.actions.githubusercontent.com
185.199.110.153			customer-stories-feed.github.com
185.199.110.154			github.githubassets.com
140.82.112.21			central.github.com
140.82.113.21			viewscreen.githubusercontent.com
185.199.110.133			desktop.githubusercontent.com
185.199.110.133			raw.github.com
185.199.108.133			repository-images.githubusercontent.com
185.199.108.153			assets-cdn.github.com
185.199.108.133			github.map.fastly.net
52.217.202.241			github-production-release-asset-2e65be.s3.amazonaws.com
52.217.198.97			github-production-repository-file-5c1aeb.s3.amazonaws.com
52.216.216.89			github-production-user-asset-6210df.s3.amazonaws.com
185.199.108.133			camo.githubusercontent.com
185.199.111.133			github.map.fastly.net
151.101.65.194			github.global.ssl.fastly.net
185.199.111.133			gist.githubusercontent.com
140.82.112.30			githubapp.com
192.0.66.2			github.blog
52.217.202.241			github-cloud.s3.amazonaws.com
185.199.111.153			githubstatus.com
185.199.109.153			guides.github.com
140.82.113.18			help.github.com
140.82.114.17			github.community
140.82.116.4			gist.github.com
185.199.111.153			github.io
140.82.116.3			github.com
192.0.66.2			github.blog
140.82.116.5			api.github.com
185.199.110.133			raw.githubusercontent.com
185.199.110.153			archiveprogram.github.com
185.199.109.153			assets-cdn.github.com
185.199.108.133			user-images.githubusercontent.com
185.199.109.133			favicons.githubusercontent.com
185.199.110.133			avatars5.githubusercontent.com
185.199.111.133			avatars4.githubusercontent.com
185.199.111.133			avatars3.githubusercontent.com
185.199.109.133			avatars2.githubusercontent.com
185.199.108.133			avatars6.githubusercontent.com
185.199.110.133			avatars7.githubusercontent.com
185.199.110.133			avatars8.githubusercontent.com
185.199.111.133			avatars1.githubusercontent.com
185.199.109.133			avatars0.githubusercontent.com
185.199.110.133			avatars.githubusercontent.com
185.199.110.133			cloud.githubusercontent.com
140.82.112.21			central.github.com
140.82.116.9			codeload.github.com
54.231.172.17			github-cloud.s3.amazonaws.com
3.5.30.161			github-com.s3.amazonaws.com
52.217.198.97			github-production-release-asset-2e65be.s3.amazonaws.com
52.217.198.97			github-production-user-asset-6210df.s3.amazonaws.com
52.217.47.84			github-production-repository-file-5c1aeb.s3.amazonaws.com
185.199.110.153			githubstatus.com
140.82.114.17			community.github.com
20.99.227.183			github.dev
185.199.110.133			media.githubusercontent.com
#github End
# Last Update Time : 2024-11-30 14:41:44 

#steam Start
23.59.200.146			steamcommunity.com
104.89.226.113			www.steamcommunity.com
104.89.226.113			steampowered.com
104.89.226.113			steamgames.com
23.192.228.231			clientconfig.akamai.steamstatic.com
103.28.54.162			ext3-hkg1.steamserver.net
23.67.33.76			test.steampowered.com
47.89.140.74			steamcloud-hkg.oss-accelerate.aliyuncs.com
193.108.88.128			ipv6check-udp.steamserver.net
23.67.33.105			steamuserimages-a.akamaihd.net
183.61.168.7			steamuserimages-a.xxghh.biz
219.152.87.117			dl.steam.clngaa.com
23.59.200.146			steamcommunity.com
23.67.33.103			steamcommunity-a.akamaihd.net
23.37.17.175			store.steampowered.com
23.59.200.146			api.steampowered.com
198.49.23.144			steampoweredmedia.com
23.59.200.146			help.steampowered.com
23.67.33.97			store.akamai.steamstatic.com
23.192.228.228			steamcdn-a.akamaihd.net
23.67.33.90			steamstore-a.akamaihd.net
104.89.226.113			steam-chat.com
23.67.33.77			community.akamai.steamstatic.com
151.101.67.52			shared.steamstatic.com
151.101.3.52			clan.steamstatic.com
23.67.33.103			cdn.steamcommunity.com
23.192.228.231			cdn.steampowered.com
23.67.33.97			cdn.store.steampowered.com
23.67.33.86			media.steampowered.com
#steam End
# Last Update Time : 2024-11-30 14:41:45 

#Ubisoft_download Start
23.40.25.65			static3.cdn.Ubi.com
23.37.17.207			static2.cdn.Ubi.com
193.108.91.206			static1.cdn.Ubi.com
#Ubisoft_download End
# Last Update Time : 2024-11-30 14:41:45 

#docker Start
141.193.213.21			docker.com
54.236.113.205			auth.docker.io
54.156.140.159			hub.docker.com
18.155.202.44			docs.docker.com
104.19.168.24			login.docker.com
54.227.20.253			registry.hub.docker.com
52.44.227.212			docker.io
54.236.113.205			registry-1.docker.io
54.227.20.253			index.docker.io
#docker End
# Last Update Time : 2024-11-30 14:41:45 

#Brave browser Start
18.164.174.129			brave.com
151.101.65.32			laptop-updates.brave.com
#Brave browser End
# Last Update Time : 2024-11-30 14:41:45 

#Tor browser Start
204.8.99.146			www.torproject.org
95.216.163.36			community.torproject.org
204.8.99.144			blog.torproject.org
#Tor browser End
# Last Update Time : 2024-11-30 14:41:45 

#Tails OS Start
204.13.164.63			tails.net
204.13.164.63			download.tails.net
#Tails OS End
# Last Update Time : 2024-11-30 14:41:45 

#Encrypt DNS Start
217.160.156.119			dns.oszx.co
172.64.41.4			mozilla.cloudflare-dns.com
172.67.153.195			0ms.dev
45.90.30.0			anycast.dns.nextdns.io
104.16.132.229			dns.cloudflare.com
146.112.41.2			doh.opendns.com
####			kaitain.restena.lu
137.66.7.89			max.rethinkdns.com
76.76.2.11			freedns.controld.com
149.248.217.117			dns.dnswarden.com
#Encrypt DNS End
# Last Update Time : 2024-11-30 14:41:46 

#EA Start
23.37.16.177			www.ea.com
23.46.216.93			origin-a.akamaihd.net
23.37.17.93			pl.ea.com
23.56.118.226			media.contentapi.ea.com
23.37.17.93			nds-network-nav.ea.com
#EA End
# Last Update Time : 2024-11-30 14:41:46 

#gitlab Start
172.65.251.78			gitlab.com
172.65.251.78			www.gitlab.com
104.17.72.206			page.gitlab.com
104.18.39.11			packages.gitlab.com
104.18.249.37			support.gitlab.com
104.18.39.11			customers.gitlab.com
172.65.216.50			staging.gitlab.com
216.198.53.1			federal-support.gitlab.com
35.227.35.254			registry.gitlab.com
172.64.35.157			evelup.gitlab.com
172.64.148.245			chef.gitlab.com
#gitlab End
# Last Update Time : 2024-11-30 14:41:46 

#debian Start
151.101.2.132			deb.debian.org
#debian End
# Last Update Time : 2024-11-30 14:41:46 

#iwara Start
104.26.12.96			iwara.tv
62.210.173.23			himeko.iwara.tv
104.26.13.96			i.iwara.tv
104.26.13.96			www.iwara.tv
66.165.237.254			hime.iwara.tv
163.172.40.145			aku.iwara.tv
163.172.42.175			sukone.iwara.tv
151.115.90.2			acheron.iwara.tv
163.172.81.17			xin.iwara.tv
163.172.40.123			uta.iwara.tv
192.211.62.190			mikoto.iwara.tv
163.172.42.175			sukone.iwara.tv
66.165.240.196			service.iwara.tv
163.172.44.153			miki.iwara.tv
104.26.12.96			api.iwara.tv
66.165.240.194			files.iwara.tv
151.115.97.15			bronya.iwara.tv
151.115.97.14			blade.iwara.tv
151.115.90.15			clara.iwara.tv
51.158.63.130			swan.iwara.tv
163.172.57.37			piko.iwara.tv
163.172.62.89			momo.iwara.tv
163.172.39.227			cul.iwara.tv
151.115.90.24			robin.iwara.tv
62.210.95.208			bailu.iwara.tv
62.210.173.23			himeko.iwara.tv
151.115.89.180			firefly.iwara.tv
151.115.97.4			lynx.iwara.tv
51.159.223.77			silverwolf.iwara.tv
62.210.173.43			pela.iwara.tv
151.115.89.253			jade.iwara.tv
151.115.97.11			welt.iwara.tv
151.115.96.228			asta.iwara.tv
151.115.90.6			sparkle.iwara.tv
151.115.90.3			yukong.iwara.tv
163.172.40.81			tei.iwara.tv
151.115.97.13			topaz.iwara.tv
151.115.90.14			kafka.iwara.tv
151.115.90.4			herta.iwara.tv
151.115.97.5			hook.iwara.tv
163.172.80.31			uni.iwara.tv
151.115.90.5			hanya.iwara.tv
#iwara End
# Last Update Time : 2024-11-30 14:41:46 

#EPIC Start
108.138.246.42			download2.epicgames.com
18.155.192.124			download3.epicgames.com
3.169.183.34			download4.epicgames.com
18.155.202.3			download.epicgames.com
23.46.216.86			epicgames-download1.akamaized.net
3.168.86.104			epic-social-social-modules-prod.ol.epicgames.com
44.219.24.124			eulatracking-public-service-prod06.ol.epicgames.com
18.155.192.86			media-cdn.epicgames.com
23.40.25.134			static-assets-prod.epicgames.com
104.100.76.60			store-content.ak.epicgames.com
54.227.239.33			tracking.epicgames.com
#EPIC End
# Last Update Time : 2024-11-30 14:41:47 

#google Start
142.251.214.131			update.googleapis.com
142.251.46.234			translate-pa.googleapis.com
142.250.189.206			translate.google.com
142.251.46.234			firebaseinstallations.googleapis.com
142.250.191.74			infinitedata-pa.googleapis.com
142.250.72.202			geller-pa.googleapis.com
108.177.104.188			alt1.mobile-gtalk.l.google.com
142.250.152.188			alt2.mobile-gtalk4.l.google.com
172.253.113.188			alt3.mobile-gtalk.l.google.com
173.194.77.188			alt4.mobile-gtalk4.l.google.com
173.194.219.188			alt5.mobile-gtalk.l.google.com
142.250.112.188			alt6.mobile-gtalk4.l.google.com
172.217.197.188			alt7.mobile-gtalk.l.google.com
108.177.12.188			alt8.mobile-gtalk4.l.google.com
142.250.189.234			translate.googleapis.com
142.250.189.206			www3.l.google.com
142.251.32.35			services.googleapis.cn
142.250.189.238			play-fe.googleapis.com
142.251.214.150			play-lh.googleusercontent.com
216.239.38.223			play.googleapis.com
108.177.104.188			alt1-mtalk.google.com
142.250.152.188			alt2-mtalk.google.com
172.253.113.188			alt3-mtalk.google.com
173.194.77.188			alt4-mtalk.google.com
173.194.219.188			alt5-mtalk.google.com
142.250.112.188			alt6-mtalk.google.com
172.217.197.188			alt7-mtalk.google.com
108.177.12.188			alt8-mtalk.google.com
142.250.189.202			content-autofill.googleapis.com
172.217.12.99			googlecn-lopri.l.google.com
142.250.189.227			www.googleapis.cn
#google End
# Last Update Time : 2024-11-30 14:41:47 

#xbox Start
23.37.16.9			gameclipscontent-d2009.xboxlive.com
23.67.33.93			images-eds.xboxlive.com
96.16.55.22			xbl-smooth.xboxlive.com
23.37.16.9			titlehub.xboxlive.com
23.67.33.105			compass.xboxlive.com
23.37.16.9			xnotify.xboxlive.com
52.165.145.141			activityhub.xboxlive.com
23.37.16.9			images-eds-ssl.xboxlive.com
199.46.35.120			rta.xboxlive.com
23.37.16.9			peoplehub.xboxlive.com
52.242.98.79			editorial.xboxlive.com
23.44.229.229			assets1.xboxlive.cn
23.44.229.229			assets2.xboxlive.cn
20.112.250.133			xboxlive.com
13.107.246.69			da.xboxservices.com
52.156.99.28			device.auth.xboxlive.com
#xbox End
# Last Update Time : 2024-11-30 14:41:47 

#Apkpure Start
172.67.20.93			download.pureapk.com
104.22.9.141			api.pureapk.com
104.22.43.111			t.apkpure.net
104.22.9.141			tapi.pureapk.com
104.22.8.141			rdelivery.pureapk.com
172.67.72.204			tapi.upload.app
45.33.36.159			api.sve.cc
#Apkpure End
# Last Update Time : 2024-11-30 14:41:48 

#Microsoft Start
20.190.190.195			login.microsoftonline.com
13.85.23.206			fe3cr.delivery.mp.microsoft.com
4.154.131.229			fe2cr.update.microsoft.com
172.202.163.200			slscr.update.microsoft.com
199.232.214.172			dl.delivery.mp.microsoft.com
52.228.161.161			nav-edge.smartscreen.microsoft.com
20.190.132.105			graph.microsoft.com
23.61.213.219			go.microsoft.com
13.107.246.69			static.edge.microsoftapp.net
204.79.197.203			oneocsp.microsoft.com
4.152.133.8			nf.smartscreen.microsoft.com
20.245.230.159			wdcp.microsoft.com
52.109.0.91			officeclient.microsoft.com
40.82.255.97			api-edge.cognitive.microsofttranslator.com
204.79.197.239			edge.microsoft.com
23.37.18.97			storeedgefd.dsx.mp.microsoft.com
23.67.33.82			msedgeextensions.sf.tlu.dl.delivery.mp.microsoft.com
#Microsoft End
# Last Update Time : 2024-11-30 14:41:48 

#spotify Start
104.199.241.202			ap-gae2.spotify.com
104.154.127.247			ap-guc3.spotify.com
104.199.65.9			ap-gew1.spotify.com
34.158.1.133			ap-gew4.spotify.com
34.158.255.62			ap-gue1.spotify.com
35.186.224.24			spclient.wg.spotify.com
35.186.224.24			wg.spotify.com
35.186.224.22			gae-spclient.spotify.com
23.67.33.81			audio4-ak-spotify-com.akamaized.net
23.212.62.85			heads4-ak-spotify-com.akamaized.net
23.67.33.90			audio-ak-spotify-com.akamaized.net
23.67.33.72			audio-akp-quic-spotify-com.akamaized.net
#spotify End
# Last Update Time : 2024-11-30 14:41:48 

#scdn Start
199.232.210.248			audio-fa.scdn.co
23.67.33.93			misc.scdn.co
23.67.33.70			i.scdn.co
199.232.214.248			newjams-images.scdn.co
199.232.210.248			dailymix-images.scdn.co
199.232.210.248			thisis-images.scdn.co
199.232.214.248			charts-images.scdn.co
199.232.214.248			seeded-session-images.scdn.co
199.232.214.248			download.scdn.co
#scdn End
# Last Update Time : 2024-11-30 14:41:48 

#onedrive Start
13.107.137.11			onedrive.live.com
13.107.42.12			skyapi.onedrive.live.com
23.56.122.108			api.onedrive.live.com
#onedrive End
# Last Update Time : 2024-11-30 14:41:48 

#other Start
3.221.73.139			www.ghostery.com
52.3.133.9			ghostery.com
104.233.133.90			wap.yushuwu.cloud
13.229.32.160			apkhub.co
162.214.80.67			apkhub.org
#other End
# Last Update Time : 2024-11-30 14:41:48 

#Github: https://github.com/Clov614/SteamHostSync

```

## 激活生效
大部分情况下是直接生效，如未生效可尝试下面的办法，刷新 DNS：
1. Windows：在 CMD 窗口输入：`ipconfig /flushdns`
2. Linux 命令：`sudo nscd restart`
3. Mac 命令：`sudo killall -HUP mDNSResponder`  

## 手动配置Source.yaml文件添加新hosts  
手动下载可执行文件第一次执行后会在目录生成Source.yaml文件，可手动配置。  

```
ua : Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/100.0.4896.127 Safari/537.36
platforms:
  -
    #github :
    - github            #数组的第一个值为对应平台
    - alive.github.com  #后续值为需要解析ip地址的域名
    - live.github.com
    - github.githubassets.com
    - central.github.com
    - desktop.githubusercontent.com
    - assets-cdn.github.com
    - camo.githubusercontent.com
    - github.map.fastly.net
    - github.global.ssl.fastly.net
    - gist.github.com
    - github.io
    - github.com
    - github.blog
    - api.github.com
    - raw.githubusercontent.com
    - user-images.githubusercontent.com
    - favicons.githubusercontent.com
    - avatars5.githubusercontent.com
    - avatars4.githubusercontent.com
    - avatars3.githubusercontent.com
    - avatars2.githubusercontent.com
    - avatars1.githubusercontent.com
    - avatars0.githubusercontent.com
    - avatars.githubusercontent.com
    - codeload.github.com
    - github-cloud.s3.amazonaws.com
    - github-com.s3.amazonaws.com
    - github-production-release-asset-2e65be.s3.amazonaws.com
    - github-production-user-asset-6210df.s3.amazonaws.com
    - github-production-repository-file-5c1aeb.s3.amazonaws.com
    - githubstatus.com
    - github.community
    - github.dev
    - media.githubusercontent.com
  -
    #steam:
    - steam
    - steamcommunity.com
    - www.steamcommunity.com
    - store.steampowered.com
    - api.steampowered.com
    - help.steampowered.com
    - store.akamai.steamstatic.com
    - steamcdn-a.akamaihd.net
    - cdn.akamai.steamstatic.com
    - steam-chat.com
    - community.akamai.steamstatic.com
```
