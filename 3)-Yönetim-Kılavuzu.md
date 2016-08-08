## Yönetim Kılavuzu

MyDLP Endpoint ajanını son kullanıcı tarafına kurduktan sonra belirlenen politikalar çerçevesinde yönetim arayüzü üzerinde kurallar oluşturulur.
 
Kurallar Veri Transfer (Data Transfer) ve Veri Keşif (Data Discovery) Kuralları olarak iki çeşittir. Politikalara çok sayıda kural eklenebilir. 

### Veri Transfer Kuralı Oluşturma

Veri Transfer Kuralı oluşturmak için, "Policy" e tıklanır, Sol tarafta "Policy" altında "General Policy" seçilir. "Add" butonuna tıklanır ve kural oluşturma sihirbazı açılır. Drop-down menüden kural tipi seçilir. 

Örnek olarak web kuralı seçilir.

![](https://cloud.githubusercontent.com/assets/20702065/17469558/0dbb1586-5d3d-11e6-8bbc-48f049844c6a.png)

Kaynak olarak (Source) Network, Computer Name, Single User, Active Directory Object, Endpoint seçilebilir.

![](https://cloud.githubusercontent.com/assets/20702065/17469559/0ff1fd74-5d3d-11e6-9bf8-40069b627b72.png)
![](https://cloud.githubusercontent.com/assets/20702065/17469562/14c72c16-5d3d-11e6-8198-13bdfbada734.png)

Hedef (Destination) seçilir.

![](https://cloud.githubusercontent.com/assets/20702065/17469563/175a59ee-5d3d-11e6-8659-f9d7d97c0269.png)

İzlenecek veri tipi seçilir. 

![](https://cloud.githubusercontent.com/assets/20702065/17469564/19d22382-5d3d-11e6-9890-3cf46e6ddba4.png)

Veri sızıntısı tespit edildiğince alınacak aksiyon seçilir ve kural kaydedilir.
![](https://cloud.githubusercontent.com/assets/20702065/17469566/1c4f506c-5d3d-11e6-84aa-5d0840ae24a2.png)

Kural ekleme tamamlandıktan sonra ana ekranda sağ üst köşede bulunan "İnstall Policy" e tıklanarak değişikliklerin uygulanması sağlanır. 
![](https://cloud.githubusercontent.com/assets/20702065/17470898/bb54b656-5d48-11e6-910d-f00233f79105.png)

Bu yöntemle istenen tüm kurallar eklenebilir. 
Daha fazla örnek bir sonraki bölümde gösterilmiştir. 

MyDLP yönetim politikalarında çok sayıda kural tipi bulunmaktadır. Aşağıda bu kuralların kullanım amaçları açıklanmıştır.

**1.	Web Kuralları:**  Ağınıza doğru veya ağınızdan geçen tüm HTTP ve HTTPS trafiğini izler ve kontrol eder. 

**2.	Mail Kuralları:** Email ve diğer SMTP trafiğini izler ve kontrol eder.  

**3.	Removable Storage Kuralları:** USB hafıza çubukları, çıkarılabilir hard disklerine transfer edilen verileri kontrol eder. 

**4.	Removable Storage Inbound Kuralları:** Son kullanıcıların çıkarılabilir medyalarından okunan dosya ve verileri kontrol eder.  

**5.	Screenshot Kuralları:** Gizli ve hassas verinin bulunduğu ekranların ekran görüntüsünün alınmasını önler. 

**6.	Printer Kuralları:**  Hassas ve gizli verilerin çıktısının alınmasını kontrol eder. 

**7.	CD-DVD Kuralları:** Seçilen kaynak bilgisayarlara takılan CD/DVD gibi optik disklerine yazılan veriyi kontrol eder.

**8.	Clipboard Kuralları:** Seçilen kaynak bilgisayarlar üzerinde kopyala yapıştır işlemlerini kontrol eder. 

**9.	API Kuralları:** MyDLP API ile MyDLP başka uygulamalarla entegre edilebilir. API kuralları ile MyDLP API nin davranışı yönetilir. 

**10.	Removable Storage Encryption Kuralları:** Ağdaki son kullanıcı makinelerine bağlanan çıkarılabilir aygıtların şifrelenmesini sağlar.

### Veri Keşif Kuralı Oluşturma

Veri Keşif kuralları ile kritik ve hassas veri içeren dosyalar keşfedilebilir. Hedefler, keşif zamanı, aranacak bilgi ve alınacak aksiyon keşif kurallarında belirlenebilir.  

Keşif Kuralı oluşturmak için "Policy" e tıklanır ve sol taraftaki menüden "Discovery Policy" seçilir. 

![](https://cloud.githubusercontent.com/assets/20702065/17469902/61527970-5d40-11e6-8d58-0ab44dd732c7.png)

Keşif yapılacak hedef seçilir. 

![](https://cloud.githubusercontent.com/assets/20702065/17469903/62b21b18-5d40-11e6-8b1b-5f3d6d1726f3.png)

Alınacak aksiyon belirlenerek kural kaydedilir.

![](https://cloud.githubusercontent.com/assets/20702065/17469907/64278adc-5d40-11e6-8b74-ba3d99e31e8d.png)