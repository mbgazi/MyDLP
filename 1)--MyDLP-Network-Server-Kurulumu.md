##MyDLP Çözümü
MyDLP ağ ve son kullanıcı tarafından kritik ve gizli verilerin dışarıya çıkmasını önlemeyi amaçlayan bir veri sızıntısı önleme çözümüdür. Daha önce open source olan ürün Comodo tarafından satın alınmıştır.
MyDLP çözümünün network server ve endpoint olmak üzere iki yazılımı bulunmaktadır. Aşağıdaki adresten bu yazılımlar indirilebilir.
[https://www.mydlp.com/getting-started/#download](https://www.mydlp.com/getting-started/#download)
## MyDLP Network Server Kurulumu
MyDLP Network Server, iç ağdan dışarıya kritik ve gizli verilerin çıkışını tespit edip önler. Ayrıca ürünün yönetimi de burdan yapılır. 
MyDLP Network Server programı fiziksel veya sanal makineye kurulabilir. Kurulacak makineler en az aşağıdaki özelliklere sahip olmalıdır:
### MyDLP Network Server System Gereksinimleri:
* Dual veya quad core Intel Xeon processors 
* En az 4GB RAM
* 256 GB veya daha fazla disk alanı
* NIC 1000/100,
* Veya bu özellikleri sağlayan sanal makine 

Ürün yukarıdaki linkten indirilir ve kurulum için aşağıdaki adımlar izlenir: 

1.	İndirilen yazılım .iso formatındadır. 
2.	Fiziksel makineye kurulacaksa .iso dosyası bir CDROM/DVDROM a yazılmalıdır.
3.	Sanal makineye kurulacaksa işletim sistemi Ubuntu 64 olan boş bir sanal makine oluşturulur. 
4.	Sanal makinenin kurulumu için CDROM/DVDROM seçeneği seçilir. 
5.	Yukarıda belirtilen minimum gereksinimler sağlanarak sanal makinenin disk, RAM vb. ayarları yapılandırılır.
6.	Sanal makinenin network ayarları “bridge mode” seçilir.
7.	Kurulum dili olarak İngilizce seçilir. 
8.	"Install MyDLP Appliance" seçilir. 
9.	Dil seçilir.
10.	Ülke seçilir.
11.	Klavye tespit seçeneği için "Hayır" seçilir. 
12.	Klavye "origin USA" seçilir.
13.	Klavye layout "USA" seçilir.
14.	Zaman dilimini kontrol et ve düzelt. 
15.	Otomatik kurulum adımları için bekle. 
16.	"OS user name" i belirle. 
17.	"OS user password" u belirle.
18.	"Encrypt home directory" seçeneği için Hayır seçilir.
19.	Otomatik kurulum adımlarını bitirmesi için bekle. 
20.	Daha sonra açılan SSH terminalinde belirlenen OS kullanıcı adı ve parola girilir.

Yukarıdaki adımlar tamamlandıktan sonra SSH terminaline;

_sudo dhclient eth0_

_ifconfig_

yazılarak IP bilgileri kontrol edilir. 
Yönetim amaçlı kullanılacak makinede bir browser açılır ve management IP si yazılarak management konsoluna giriş yapılır. 
Management konsolunun varsayılan kullanıcı adı: mydlp şifresi: mydlp Bu bilgileri kullanarak giriş yapılır ve MyDLP ürünü yönetilir. 

Deneme lisansı [https://accounts.comodo.com/account/login](https://accounts.comodo.com/account/login) adresine mail adresiyle kayıt olup, lisans talebinde bulunulur. Emaile gelen doğrulama kodunu doğrulattıktan sonra lisans bilgisi elde edilir. 
![](https://cloud.githubusercontent.com/assets/20702065/17457902/4a582366-5c0d-11e6-9a03-c1d484107774.png)
![](https://cloud.githubusercontent.com/assets/20702065/17457913/5e91fa3c-5c0d-11e6-900b-9b68f72c204e.png)

Daha sonra MyDLP yönetim arayüzüne bağlanıp, aşağıdaki ekrana lisans kodu girilir ve lisansın doğrulanması beklenir.
![](https://cloud.githubusercontent.com/assets/20702065/17457919/6b0dd998-5c0d-11e6-88b6-039349ebb5a6.png)

Lisans doğrulandıktan sonra yönetim arayüzü politikaları belirlemek için hazır hale gelir. 
<img width="1079" alt="screen shot 2016-07-30 at 19 39 49" src="https://cloud.githubusercontent.com/assets/20702065/17458000/9605bb60-5c0e-11e6-8a9b-1eb947c69435.png">
