Bu bölümde çok sayıda örnek MyDLP Yönetim Politikası oluşturulmuş, son kullanıcıda bu kuralların nasıl test edileceği gösterilmiş ve testler sonucu MyDLP Yönetim Konsolunda oluşan loglar, alınan aksiyonlar gösterilmiştir. 

# Web Kuralı (Kredi Kartı Bilgisi İzleme)
* MyDLP Server Yönetim Arayüzüne bağlanılır. 
* Policy/General Policy'ye tıklanır. Add butonuna basılır. Kural oluşturma sihirbazı başlar.
* "Web Rules" seçilir, kuralın adı yazılır..

![](https://cloud.githubusercontent.com/assets/20702065/17469558/0dbb1586-5d3d-11e6-8bbc-48f049844c6a.png)

* Kaynaklar seçilir.

![](https://cloud.githubusercontent.com/assets/20702065/17469559/0ff1fd74-5d3d-11e6-9bf8-40069b627b72.png)

![](https://cloud.githubusercontent.com/assets/20702065/17469562/14c72c16-5d3d-11e6-8198-13bdfbada734.png)

* Hedefler seçilir.

![](https://cloud.githubusercontent.com/assets/20702065/17469563/175a59ee-5d3d-11e6-8659-f9d7d97c0269.png)

* İncelenecek veriler seçilir.

![](https://cloud.githubusercontent.com/assets/20702065/17469564/19d22382-5d3d-11e6-9890-3cf46e6ddba4.png)

* Alınacak aksiyon seçilir.

![](https://cloud.githubusercontent.com/assets/20702065/17469566/1c4f506c-5d3d-11e6-84aa-5d0840ae24a2.png)

* Son kullanıcı makinesinde bir internet tarayıcısı açılır. dlptest.com adresine gidilerek, deneme postları yapılabilir, örnek (sample) veri alınabilir. 

![](https://cloud.githubusercontent.com/assets/20702065/17470895/b8089490-5d48-11e6-99fb-c900b6e7de36.png)

* Sample Data sekmesindeki kredi kartı numaralarından bir kaçı post edilir.

![](https://cloud.githubusercontent.com/assets/20702065/17470896/b9d62b66-5d48-11e6-89d3-7ea91a8ff38b.png)

* MyDLP Server Yönetim Arayüzünde Loglar sekmesine tıklanır. Burada kredi kartı gönderme bilgisinin loglara düşüp düşmediği kontrol edilir. 

![](https://cloud.githubusercontent.com/assets/20702065/17470901/bed4f340-5d48-11e6-93c9-613fd9adfd9d.png)
![](https://cloud.githubusercontent.com/assets/20702065/17470904/c0733202-5d48-11e6-9747-d881ab26228f.png)

# Printer Kuralı Oluşturmak
* MyDLP Server Yönetim Arayüzüne bağlanılır. 
* Policy/General Policy'ye tıklanır. Add butonuna basılır. Kural oluşturma sihirbazı başlar.
* Printer kural tipi seçilir. 

![](https://cloud.githubusercontent.com/assets/20702065/17469607/5b6e4406-5d3d-11e6-9516-0254e047c57c.png)

* Kaynaklar seçilir.
* Hedefler seçilir. 
* İncelenecek veri tipi olarak kredi kartı bilgisi seçilir.
* Aksiyon olarak "Block" seçilir.

![](https://cloud.githubusercontent.com/assets/20702065/17469572/26885cd6-5d3d-11e6-9fc7-78ad65fb9ac3.png)

* Son kullanıcı makinesinde bir notepad açılır. Kredi kartı numaraları yazılır. Daha sonra bu dokümanı yazdırmak denenir.

* MyDLP Endpoint Ajanının yazdırma işlemini yaptırmadığı, engellediği görülür.

![](https://cloud.githubusercontent.com/assets/20702065/17470916/cfaa5304-5d48-11e6-8f9d-0f502c4ecfb6.png)

* MyDLP Network Server Yönetim Arayüzü üzerinde logun geldiği kontrol edilir.

![](https://cloud.githubusercontent.com/assets/20702065/17470921/d1e515f0-5d48-11e6-8e85-4edb31f7a1b0.png)

# Panoya Kopyalama/Yapıştırma Kuralı 

* MyDLP Server Yönetim Arayüzüne bağlanılır. 
* Policy/General Policy'ye tıklanır. Add butonuna basılır. Kural oluşturma sihirbazı başlar.
* Clipboard kural tipi seçilir. 

![](https://cloud.githubusercontent.com/assets/20702065/17469581/2d5683a8-5d3d-11e6-9440-2234ab4aa101.png)

* Kaynaklar seçilir

![](https://cloud.githubusercontent.com/assets/20702065/17469583/2f21051e-5d3d-11e6-9068-1255f802f73d.png)

* Hedefler seçilir

* İncelenecek veri tipi olarak "Name with SSN" seçilir.
* Alınacak aksiyon seçilir. 
* Son kullanıcı makinesinde bir notepad açılır. İsim ve SSN (Social Security Number) yazılır. Daha sonra bu bilgileri kopyalayıp yapıştırmak denenir ve yönetim arayüzünde logun geldiğinden emin olunur.

![](https://cloud.githubusercontent.com/assets/20702065/17470909/c629b612-5d48-11e6-83a5-4c0c4e3dc85d.png)

# Web Kuralı Oluşturma (keyword) 

* MyDLP Server Yönetim Arayüzüne bağlanılır. 
* Policy/General Policy'ye tıklanır. Add butonuna basılır. Kural oluşturma sihirbazı başlar.
* "Web Rules" seçilir, kuralın adı yazılır.

![](https://cloud.githubusercontent.com/assets/20702065/17469595/454e9bc6-5d3d-11e6-8a71-066704c545a2.png)

* Sırasıyla Kaynaklar, Hedefler seçilir. 

* İncelenecek veri tipleri seçilir.

![](https://cloud.githubusercontent.com/assets/20702065/17469601/5113492a-5d3d-11e6-8c32-072125fef137.png)

* Alınacak aksiyon olarak Log seçilir.

![](https://cloud.githubusercontent.com/assets/20702065/17469594/3fe5beee-5d3d-11e6-87ab-72b36b0f820e.png)

* Son kullanıcı makinesinde bir internet tarayıcısı açılır. dlptest.com adresine gidilerek, seçilen keywordler yazılarak post edilir.

![](https://cloud.githubusercontent.com/assets/20702065/17470892/b42811f2-5d48-11e6-976e-a4376cf74c33.png)

* MyDLP Server Yönetim Arayüzünde Loglar sekmesine tıklanır. Burada keyword kuralın tetiklediği logların oluşup oluşmadığı kontrol edilir. 

![](https://cloud.githubusercontent.com/assets/20702065/17470481/646d7d26-5d45-11e6-8c11-b8a12cdf1efe.png)