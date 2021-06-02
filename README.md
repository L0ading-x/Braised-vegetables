# Braised-vegetables
将hw时信息收集以及简单的漏洞扫描操作步骤简单化
使用subfinder(被动子域名爆破收集) subdomain(主动域名爆破) nabbu(端口扫描) httpx(探测目录浏览) crawlergo(360深度爬虫) chorme(谷歌浏览器) xray(漏洞扫描) dirsearch(扫描目录) server酱(微信漏洞消息提醒)将收集步骤简单化。
希望师父们多多给star。

#how to use?
run it by cmd
subfinder -dL test.txt -o subfinder.txt -silent|ksubdomain -verify -summary -o ksubdomain.txt -silent|naabu -exclude-cdn -o naabu.txt -silent|httpx -silent > targets.txt && python launcher.py && copy targets.txt C:\Users\Administrator\Desktop\crawlergo_x_XRAY-master\crawlergo_x_XRAY-master\crawlergo\dirsearch-master && cd dirsearch-master && python dirsearch.py -l targets.txt -e *
