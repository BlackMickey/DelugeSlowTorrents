# DelugeControlforU2
U2 專用的 Deluge 1.3.15 客戶端上傳速度控制器  
(本腳本由 **DelugeSlowTorrents** 修改而來)  
<br/>  

U2 有最大有效上傳速度限制，如果匯報時，平均上傳速度超過該速度時，本次匯報的上傳與下載均不列入計算，此腳本實時計算剩餘的流量，執行動態上傳速度控制，盡可能不浪費任何一點上傳量。

############### 安裝與執行 ###############

安裝
> apt install screen  
> mv -f commands /usr/lib/python2.7/dist-packages/deluge-1.3.15-py2.7.egg/deluge/ui/console/commands  
> 修改 DelugeControlforU2.pl 參數設定

執行
> screen -dmS DelugeControlforU2  
> screen -r DelugeControlforU2  
> perl DelugeControlforU2.pl  



靈感來源  
https://www.reddit.com/r/seedboxes/comments/b37h8k/scripthowto_automatically_delete_slow_torrents/
