## MyDLP Endpoint Agent Kurulumu

MyDLP Endpoint ilgili ağdaki tüm son kullanıcı bilgisayarlarına kurulmalı ve belirlenen politikalar bu bilgisayarlar üzerinde uygulanmalıdır. Böylece son kullanıcı tarafından kritik ve hassas verilerin ağ dışına çıkarılması izlenip, engellenebilir.

MyDLP Endpoint kurulmadan önce MyDLP Network Server kurulmalıdır. MyDLP Network Server'ın yönetim arayüzünden MyDLP Endpoint ajanları yönetilebilir. 

### MyDLP Endpoint Ajanı Gereksinimleri:
* Windows XP, Windows 7, Windows 8, Windows 10, Windows Server 2003, Window Server 2008 işletim sistemi(64 bit /32 bit)
* 1GB RAM
* En az 200 MB boş disk alanı 

### Son Kullanıcı Makinesinde MyDLP Endpoint Ajanı Kurulum Adımları
1. MyDLP Server Yönetim Konsolunda Settings/Protocols altında Downloads bölümünden MyDLP Agent ına tıklayarak .msi uzantılı dosya indirilir.
2. Kuruluma başlamadan önce MyDLP Serverına SSH ile bağlanıp "Configuration Script" inde aşağıdaki değişiklikler yapılır.

  * "nano /usr/share/mydlp/endpoint/win/mydlp-dep-conf.vbs" komutu yazılarak “.conf” dosyası açılır
  * 10.0.0.2 IP si MyDLP Server IP si ile değiştirilir.  MYDLP_SERVER=”sizimserverIPniz”
  * İkinci satırdaki mydlp de server IP si ile değiştirilir. 
  * MYDLP_SHARE=”\\SİZİNSERVERIPniz\downloads”
  * CTRL+X ve Y ye basılarak dosyadan çıkılır. 
!!!!!!!!!!!!!EKRAN ÇIKTISI KOYYYYYYY**
3. Kuruluma başlamadan önce ayrıca bağlı paketlerin kurulumu aşağıdaki adımlar izlenerek gerçekleştirilir.
MyDLP Serverına SSH ile bağlanılır.

  * "sudo mydlp-download-xp-deps" komutu yazılır.
  * İlgili bağlı dosyalar /usr/share/mydlp/endpoint/deps/ dizinine indirilir.

!!!!!!!!!!!!!!EKRAN ÇIKTISI KOYYYYYYY**

4. MyDLP Endpoint ajanı server üzerindeki "\\mydlpserverip\downloads" dosyadan veya 1. maddedeki yöntem ile indirilir.

5. Son kullanıcı makinede endpoint agent .msi uzantılı dosyaya tıklanarak kurulum sihirbazı açılır.

![](https://cloud.githubusercontent.com/assets/20702065/17460715/d84371e0-5c7a-11e6-9e1b-262a28f2b7d8.png)

![](https://cloud.githubusercontent.com/assets/20702065/17460716/dc2fa6e8-5c7a-11e6-94c7-71eb542529de.png)
6. MyDLP Server IP adresi girilir ve "next" ile devam edilir.

![](https://cloud.githubusercontent.com/assets/20702065/17460717/de8f03de-5c7a-11e6-9a4b-600ddfe5c7ba.png)
7. Kurulum tamamlanır ve "Finish" e tıklanır.

![](https://cloud.githubusercontent.com/assets/20702065/17460723/fb53d6c0-5c7a-11e6-9040-ff4d3a35b8ba.png)
8. MyDLP Server Yönetim Konsoluna gidilir, Endpoints sekmesine tıklanır ve kurulan endpoint ajanının eklendiğinden emin olunur.

![](https://cloud.githubusercontent.com/assets/20702065/17460731/1375fc7e-5c7b-11e6-9795-1ead1fd2943e.png)

## Proxy Ayarları

Endpoint ajanı kurulduktan ve MyDLP Server Yönetim Konsolunda bu ajan görüldükten sonra son kullanıcının ağ isteklerinin MyDLP Serverından geçmesi için kullanıcının Proxy ayarlarının değiştirilmesi, Proxy Server olarak MyDlp Server ın IP si verilmelidir.

Her web tarayıcısında proxy ayarları farklı yöntemlerle yapılandırılır. Örnek olarak Internet Explorer yapılandırılması aşağıdaki gibi gerçekleştirilir. Diğer tarayıcılar için benzer adımlar uygulanabilir.
 * Internet Expolorer üzerinde Seçenekler den Bağlantılar sekmesine tıklanır.
   
   ![](https://cloud.githubusercontent.com/assets/20702065/17460733/1a394df4-5c7b-11e6-80e0-82ae436c0a31.png)
 * LAN Settings e tıklanır.
 * Proxy Server olarak MyDLP Serverın IPsi yazılır, port olarak da 3128 yazılır. 
  
   ![](https://cloud.githubusercontent.com/assets/20702065/17460734/1d063592-5c7b-11e6-9347-a1cbd080889f.png)
 
Proxy ayarları da yapıldıktan sonra MyDLP Server Yönetim Konsolundan gerekli politikalar oluşturularak MyDLP ajanı kurulu son kullanıcılar izlenir ve veri  transferlerinde gerekli aksiyonlar (Geçir, Engelle, Logla, Karantinaya Al vb.) alınır.

