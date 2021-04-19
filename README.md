#Homework-Proxylogon事件討論

甚麼是Proxylogon事件:
Proxylogon事件是由一個中國政府支持的駭客組織Hafnium，利用Exchange Server的4項零時差漏洞對本地部署郵件系統所進行的駭客攻擊，編號名為「CVE-2021-26855 」及「CVE-2021-27065」（稱其為「ProxyLogon」）並由一個台灣的資安研究團隊「戴夫寇爾」於2020年12月10日發現。


Proxylogon事件所造成影響:
由於Proxylogon攻擊是針對攻擊是針對微軟的Exchange Server進行的攻擊，駭客利用這些漏洞來存取企業內的 Exchange 伺服器，駭入使用者的電子郵件帳號，並且安裝其他惡意程式包含Web Shell、DearCry(勒索軟體)、Black Kingdom(勒索軟體)、DLTMiner(挖礦程式)等等的嚴重影響各個公司、國家機密資料與一般電腦使用者的安全。雖然目前絕大多數本地部署的Exchange Server都已經修補好ProxyLogon漏洞，但微軟警告，這不表示事情就做完了，因為許多一開始被駭而不自知的企業，有許多未爆彈得解決，如駭客滲透進企業網路，或是以偷來的帳密駭入其他系統。



防範方法:
微軟建議企業應立即檢視Exchange Server是否有駭入跡象、web shell，並檢查用戶及用戶群組是否有可疑新增帳號，呼籲變更所有用戶帳號和本地管理員帳號密碼，而 Event ID 1102則意味駭客刪除事件log。另外也要留心滲透手法，如RDP、防火牆、WMI訂閱及WinRM組態可疑變更、新增的服務、排程或啟動物件，或是非微軟的RDP及遠端存取，以及不明的Exchange郵件轉寄政策變更等。
