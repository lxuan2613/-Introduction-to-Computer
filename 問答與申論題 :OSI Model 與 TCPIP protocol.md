 # 問答與申論題 :OSI Model 與 TCP/IP protocol
 
1.解釋 communication protocol(簡稱協定 protocol) ： Communications Protocol：通信協定一種大家所認同的方法來互相溝通稱之為協議。

2. Why Layering? (為何要分層 ?)
 
 3. 列出 OSI Model 與 TCP/IP protocol對應圖
   註 1: 需用中英文寫出各層的名稱
   註 2:須說明 OSI Model每一層的簡略功能
   
 (1)
 ![image](https://github.com/lxuan2613/-Introduction-to-Computer/blob/main/TCP-IP%E6%A8%A1%E5%9E%8B%20(2).png)
 ![image]https://www.google.com/url?sa=i&url=http%3A%2F%2Flinux.vbird.org%2Flinux_server%2F0110network_basic.php&psig=AOvVaw3KO6pxl-vmh7URUPOhfnXn&ust=1605921526538000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCOCBj7f5j-0CFQAAAAAdAAAAABAc
 
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


5. TCP vs UDP
[1]英文全名
[2]須說明 reliable(可靠) vs un-reliable(不可靠)
[3]如何達到reliable(可靠)
[4]Three-way handshaking機制

6.簡述下列網路設備  主要功能 與 特色 及 運作在 OSI哪一層
(1) Hub vs Repeater
(2)Switch vs Bridge
(3)Router vs L3 Switch
(4)Proxy

7.簡述下列 簡述下列 address(位址 )的意義 與定義 在 OSI Model哪一層
(1)PORT address
(2)IP address
(3)MAC address

