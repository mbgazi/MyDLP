## Yönetim Kılavuzu

MyDLP Endpoint ajanını son kullanıcı tarafına kurduktan sonra belirlenen politikalar çerçevesinde yönetim arayüzü üzerinde kurallar oluşturulur.
 
Kurallar Veri Transfer (Data Transfer) ve Veri Keşif (Data Discovery) Kuralları olarak iki çeşittir. Politikalara çok sayıda kural eklenebilir. 

### Veri Transfer Kuralı Oluşturma

Veri Transfer Kuralı oluşturmak için, "Policy" e tıklanır, Sol tarafta "Policy" altında "General Policy" seçilir. "Add" butonuna tıklanır ve kural oluşturma sihirbazı açılır. Drop-down menüden kural tipi seçilir. 

MyDLP yönetim politikalarında çok sayıda kural tipi bulunmaktadır. Aşağıda bu kuralların kullanım amaçları açıklanmıştır.

1.	Web Kuralları: Ağınıza doğru veya ağınızdan geçen tüm HTTP ve HTTPS trafiğini izler ve kontrol eder. 
2.	Mail Kuralları: Email ve diğer SMTP trafiğini izler ve kontrol eder.  
3.	Removable Storage Kuralları: USB hafıza çubukları, çıkarılabilir hard disklerine transfer edilen verileri kontrol eder. 
4.	Removable Storage Inbound Kuralları: Son kullanıcıların çıkarılabilir medyalarından okunan dosya ve verileri kontrol eder.  
5.	Screenshot Kuralları: Gizli ve hassas verinin bulunduğu ekranların ekran görüntüsünün alınmasını önler. 
6.	Printer Kuralları: Hassas ve gizli verilerin çıktısının alınmasını kontrol eder. 
7.	CD-DVD Kuralları: Seçilen kaynak bilgisayarlara takılan CD/DVD gibi optik disklerine yazılan veriyi kontrol eder.
8.	Clipboard Kuralları: Seçilen kaynak bilgisayarlar üzerinde kopyala yapıştır işlemlerini kontrol eder. 
9.	API Kuralları: MyDLP API ile MyDLP başka uygulamalarla entegre edilebilir. API kuralları ile MyDLP API nin davranışı yönetilir. 
10.	Removable Storage Encryption Kuralları: Ağdaki son kullanıcı makinelerine bağlanan çıkarılabilir aygıtların şifrelenmesini sağlar.

Örnek olarak web kuralı seçilir.
![](https://cloud.githubusercontent.com/assets/20702065/17469558/0dbb1586-5d3d-11e6-8bbc-48f049844c6a.png)

Kaynak olarak (Source) Network, Endpoint, 
![](https://cloud.githubusercontent.com/assets/20702065/17469559/0ff1fd74-5d3d-11e6-9bf8-40069b627b72.png)
![](https://cloud.githubusercontent.com/assets/20702065/17469562/14c72c16-5d3d-11e6-8198-13bdfbada734.png)

### Veri Keşif Kuralı Oluşturma
