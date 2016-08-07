## MyDLP Endpoint Agent Kurulumu
MyDLP Endpoint ilgili ağdaki tüm son kullanıcı bilgisayarlarına kurulmalı ve belirlenen politikalar bu bilgisayarlar üzerinde uygulanmalıdır. Böylece son kullanıcı tarafından kritik ve hassas verilerin ağ dışına çıkarılması izlenip, engellenebilir.
MyDLP Endpoint kurulmadan önce MyDLP Network Server kurulmalıdır. MyDLP Network Server'ın yönetim arayüzünden MyDLP Endpoint ajanları yönetilebilir. 
### MyDLP Endpoint Agent Gereksinimleri:
* Windows XP, Windows 7, Windows 8, Windows 10, Windows Server 2003, Window Server 2008 işletim sistemi(64 bit /32 bit)
* 1GB RAM
* En az 200 MB boş disk alanı 

### Son Kullanıcı Makinesinde MyDLP Endpoint Ajanı Kurulum Adımları

1. MyDLP Yönetim Konsolunda Settings/Protocols altında Downloads bölümünden MyDLP Agent ına tıklayarak .msi uzantılı dosya indirilir.
2. Kuruluma başlamadan önce MyDLP Serverına SSH ile bağlanıp "Configuration Script" inde aşağıdaki değişiklikler yapılır.

  * "nano /usr/share/mydlp/endpoint/win/mydlp-dep-conf.vbs" komutu yazılarak “.conf” dosyası açılır
  * 10.0.0.2 IP si MyDLP Server IP si ile değiştirilir.  MYDLP_SERVER=”sizimserverIPniz”
  * İkinci satırdaki mydlp de server IP si ile değiştirilir. 
  * MYDLP_SHARE=”\\SİZİNSERVERIPniz\downloads”
  * CTRL+X ve Y ye basılarak dosyadan çıkılır. 

3. Kurulmua başlamadan önce ayrıca bağlı paketlerin kurulumu aşağıdaki adımlar izlenerek gerçekleştirilir.
MyDLP Serverına SSH ile bağlanılır.

  * "sudo mydlp-download-xp-deps" komutu yazılır.
  * İlgili bağlı dosyalar /usr/share/mydlp/endpoint/deps/ dizinine indirilir.

3.4.3. MyDLP Endpoint
Latest MyDLP Endpoint is available on MyDLP Server, you can also access via shared folder on server. To access please do
following steps;
1. Please open run on your windows client.
2. Type "\\mydlpserverip\downloads"
3. You can find latest endpoint under win folder. 
