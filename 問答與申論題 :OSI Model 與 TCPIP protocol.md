 # 問答與申論題 :OSI Model 與 TCP/IP protocol
 
1.解釋 communication protocol(簡稱協定 protocol) ： Communications Protocol：通信協定一種大家所認同的方法來互相溝通稱之為協議。

2. Why Layering? (為何要分層 ?)
 
 3. 列出 OSI Model 與 TCP/IP protocol對應圖
   註 1: 需用中英文寫出各層的名稱
   註 2:須說明 OSI Model每一層的簡略功能
   
(1)
 ![image](https://github.com/lxuan2613/-Introduction-to-Computer/blob/main/TCP-IP%E6%A8%A1%E5%9E%8B%20(2).png)
 ![image](http://linux.vbird.org/linux_server/0110network_basic//osi_tcpip.gif)
 
(2)
第一層︰實體層（Physical Layer）
實體層是OSI模型的最底層，它用來定義網路裝置之間的位元資料傳輸

第二層︰資料連結層（Data Link Layer）
資料連結層介於實體層與網路層之間，主要是在網路之間建立邏輯連結

第三層︰網路層（Network Layer）
網路層定義網路路由及定址功能，讓資料能夠在網路間傳遞

第四層︰傳輸層（Transport Layer）
傳輸層主要負責電腦整體的資料傳輸及控制

第五層︰會議層（Session Layer）
這個層級負責建立網路連線，等到資料傳輸結束時，再將連線中斷

第六層︰展示層（Presentation Layer）
應用層收到的資料後，透過展示層可轉換表達方式

第七層︰應用層（Application Layer）
應用層主要功能是處理應用程式，進而提供使用者網路應用服務

詳細： https://www.ithome.com.tw/node/47085




4. 簡述 下列協定的功能 與特色並說明它們 運作在 TCP/IP的哪一層?
   (1)HTTP vs HTTPS (2) TELNET vs SSH (3)DNS (4)IP (5)ICMP
    
(1) 應用層
HTTP 全名是 超文本傳輸協定（HyperText Transfer Protocol），內容只規範了客戶端請求與伺服器回應的標準，實際上是藉由 TCP 作為資料的傳輸方式。
HTTPS 全名 超文本傳輸安全協定，那個 S 就是 Secure 的意思；HTTPS 透過 HTTP 進行通訊，但通訊過程使用 SSL/TLS 進行加密，藉由類似於前述的加密方式，在 HTTP 之上定義了相對安全的資料傳輸方法。

(2) 應用層
telnet：執行Telnet程式來連線到遠端伺服器並輸入帳密讓使用者可以遠端控制主機。但是因為傳輸的資料並未加密所以容易遭到竊取，因此後來多改用較安全的SSH。
SSH：是在不安全的網路上進行安全遠端登入和其他安全網路服務的協定(RFC 4251)，SSH由三個主要協定組成。

(3)DNS 
DNS的全稱是Domain Name System(或Service)，是一套系統軟體，讓大家所使用及管理的電腦網路系統
DNS兩大功用
FORWARD DOMAIN(正解)：DOMAIN NAME a IP ADDRESS
REVERSE DOMAIN(反解)：IP ADDRESS a DOMAIN NAME

(4)IP 網路層
IP是英文Internet Protocol的縮寫，意思是「網絡之間互連的協議」，也就是為計算機網絡相互連接進行通信而設計的協議。
IP兩個主要的功能：
標識主機：更具體地說，標識其網路介面，並且提供主機在網路中的位置。
網路定址：網際協定（IP）的一個重要機制就是 網路定址（internet address），該功能的目的是將資料報 從一個網路模組送到目的地。


(5)ICMP 網路層
網際網路控制訊息協定（Internet Control Message Protocol）是網際網路協定套組的核心協定之一。
該協定的最主要目的，是用來解析網路封包或是分析路由的情況，大多是透過所傳回來的錯誤訊息進行分析，而網路管理人員則利用這個協定的工具來了解狀況，進而使用其他措施解決所遇到的問題。



5. TCP vs UDP
[1]英文全名
[2]須說明 reliable(可靠) vs un-reliable(不可靠)
[3]如何達到reliable(可靠)
[4]Three-way handshaking機制

5. 傳輸控制協定(Transmission Control Protocol) vs 用戶資料報協定(User Datagram Protocol)
[1]
差別在於 TCP是雙向傳輸 UDP是單向.TCP傳送東西.會有封包數據.他可靠性高UDP可靠性低.傳送東西速度快。
在 TCP/ IP 協定家族中﹐傳送層主要有兩個協定﹕TCP 與 UDP。
[2]
TCP 提供的是一個連線導向(Connection Oriented)的"可靠傳輸"﹐前面所介紹的傳送層檢測手續﹐都會在 TCP 中得到實現。

UDP 則是一個非連線型(Connectionless)的"非可靠傳輸"協定﹐它並不會運用確認機制來保證資料是否正確的被接收、不需要重傳遺失的資料、資料的接收可不必按順序進行、也不提供回傳機制來控制資料流的速度。

[3]通常在每個TCP報文段中都有一對序號和確認號。

[4]三向交握 (Three-way Handshake)， 是其建立虛擬連線 (virtual connection) 的方式。
 又稱為 三向式握手、三路交握 …，其實就是 三次訊息的交換。


6.簡述下列網路設備  主要功能 與 特色 及 運作在 OSI哪一層
(1) Hub vs Repeater
(2)Switch vs Bridge
(3)Router vs L3 Switch
(4)Proxy

(1)集線器(Hub) vs 中繼器(Repeater)
而 Hub 則常見於網路的拓樸上，有多各 port ，分別連接主機/設備或是其它 Hub 。功能上，兩者都是一樣的：中繼器(Repeater)將信號放大，再重送一遍。或許，我們可以簡單的將 hub 的每一各 port 都視為 repeater 就是了。
實體層

(2)Switch vs Bridge
Switch :  改進了 Hub 的缺點, 因為OSI-2 可以記住各個連接的電腦的 MAC傳送封包時　往目的電腦所連接的 Interface (Port) 傳送而不會每個連接埠皆傳送, 造成網路壅塞
Bridge :  簡而言之　就是只有兩個孔的 Switch 只用來連接兩個區域網路
實體層

(3)Router vs L3 Switch
Router功能類似 Bridge　和 Switch可以像Switch 連接許多電腦或是連接兩個不同的區域網路但是注意 Switch/Bridge 只能連接兩個區域網路而 Router 更可以連接多個並且建立路由表。
Layer 3 Switch 彌補Router 不足之處用在Lan的範圍內與Router互補( Inter — vlan Routing)L3 Switch 的成本相較於Router也較便宜，適合放在內部做Routing用。
速度也比較快!
實體層

(4)Proxy (代理伺服器)




7.簡述下列 簡述下列 address(位址 )的意義 與定義 在 OSI Model哪一層
(1)PORT address
(2)IP address
(3)MAC address

