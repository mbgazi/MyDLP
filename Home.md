# Welcome to the MyDLP wiki!
MyDLP ağ ve son kullanıcı tarafından kritik ve gizli verilerin dışarıya çıkmasını önlemeyi amaçlayan bir veri sızıntısı önleme çözümüdür. 
MyDLP çözümünün network server ve endpoint olmak üzere iki yazılımı bulunmaktadır. Aşağıdaki adresten bu yazılımlar indirilebilir.[https://www.mydlp.com/getting-started/#download](https://www.mydlp.com/getting-started/#download)
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
1. İndirilen yazılım .iso formatındadır. 
2. Fiziksel makineye kurulacaksa .iso bir CDROM/DVDROM a yazılmalıdır.
3. Sanal makineye kurulacaksa işletim sistemi Ubuntu 64 olan bir sanal makine oluşturulur. 
4. Sanal makinenin kurulumu için CDROM/DVDROM seçeneği seçilir. 
5. Kurulum dili olarak İngilizce seçilir. 
6. "Install MyDLP Appliance" seçilir. 
7. Dil seçilir.
8. Ülke seçilir.
9. Klavye tespit seçeneği için "Hayır" seçilir. 
9. Klavye "origin USA" seçilir.
10. Klavye layout "USA" seçilir.
11. Zaman dilimini kontrol et ve düzelt. 
12. Otomatik kurulum adımları için bekle. 
13. "OS user name" i belirle. 
14. "OS user password" u belirle.
15. "Encrypt home directory" seçeneği için Hayır seçilir.
16. Otomatik kurulum adımlarını bitirmesi için bekle. 
17. Daha sonra açılan SSH terminalinde belirlenen OS kullanıcı adı ve parola girilir.
Yukarıdaki adımlar tamamlandıktan sonra ifconfig yazılarak IP bilgileri kontrol edilir. 
Yönetim amaçlı kullanılacak makinede managemen IP si yazılarak management konsoluna giriş yapılır. 
Management konsolunun varsayılan kullanıcı adı:mydlp şifresi: mydlp 

## MyDLP Endpoint Agent Kurulumu
### MyDLP Endpoint Agent Gereksinimleri:
* Windows XP, Windows 7, Windows 8, Windows 10, Windows Server 2003, Window Server 2008 işletim sistemi(64 bit /32 bit)
* 1GB RAM
* En az 200 MB boş disk alanı 



