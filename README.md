# multithreading-in-big-data-using-Java-and-Python
 multithreading in big data using Java and Python
 NOT:
 ● Kullanılacak veri setine aşağıdaki linkten ulaşabilirsiniz:
https://www.kaggle.com/datasets/selener/consumer-complaint-database

 A.PROJE HAKKINDA
Müşteri şikayetleri kayıtlarının tutulduğu bir veri seti içerisindeki benzer kayıtlar tespit
edilecek ve tespit edilen kayıtlar masaüstü uygulamasında gösterilecektir. Multithreading
kullanarak benzerlik arama süresini düşürmek amaçlanmaktadır.
Amaç:
1. Veri seti içerisindeki arama işlem süresini multithreading kullanılarak azaltmak.
2. Belirtilen sütun/sütunlar için her bir satırdaki kayıtların birbiriyle kelime bazlı
karşılaştırılması ve aralarındaki benzerliğin tespit edilmesi.
3. Uygulama içerisinde istenen özelliklere göre kayıtları filtrelemek ve kullanıcıya
göstermek.
4. Masaüstü uygulama geliştirme hakkında bilgi ve beceriye sahip olmak

 Veri seti aşağıdaki kurallara uygun olacak şekilde yeniden düzenlenmelidir:
○ Elde edilen tabloda 6 farklı sütun bulunmalıdır: Product (Ürün), Issue (Konu),
Company (Şirket), State, Complaint ID, Zip Code.
○ Null değer içeren kayıtlar bulunmamalıdır.
○ Kayıtlardaki noktalama işaretleri kaldırılmalıdır.
○ Kayıtlardaki stop word’ler kaldırılmalıdır (nltk kütüphanesi kullanılabilir).

Benzerlik Tespiti:
Geliştirilecek projede tüm kayıtlar arasındaki benzerlik ilişkisinin incelenmesi beklenmektedir.
Bu nedenle her bir kaydın diğer bir kayıtla karşılaştırılması gerekmektedir. Karşılaştırmanın
mümkün olduğunca hızlı olması için multithread kullanılmalıdır. Benzerlik, kayıtların
içerdikleri ortak kelime sayısına göre olmalıdır

PROJEDE YAPTIKLARIM:
1. Verilen veri seti istenen şekilde yeniden düzenlenmelidir.
2. Düzenlenmiş veri setindeki kayıtlar arasında benzerlik kontrolü yapılmalıdır. Kontrol
sırasında mutlaka multithreading kullanılmalıdır. Multithreading için kullanılacak
thread sayısı uygulama arayüzünden girilmelidir.
3. Her thread’in çalışma zamanı ve tüm thread’ler için toplam çalışma zamanı bilgileri
uygulama arayüzünde gösterilmelidir.
4. İstenilen sütun ya da sütunlar arasındaki girilen benzerlik oranı (threshold) ve üzerinde
benzerliğe sahip kayıtlar masaüstü uygulamasında gösterilmelidir.
5. Uygulamanızı sunmak üzere basit bir arayüz geliştirmeniz istenmektedir. Bu arayüz
aşağıdaki isterleri içermelidir:
• Benzerlik oranının (Threshold değeri) seçilebileceği / girilebileceği bir araç,
• Benzerliklerinin araştırılması istenen sütun veya sütunların seçilebileceği bir
araç,
• Kaç tane thread kullanılacağının seçilebileceği / girilebileceği bir araç,
• Her bir thread’in çalışma zamanını ve toplam çalışma zamanını gösteren araçlar
• Sonuçların açıkça ekranda gösterilebileceği bir araç.
6. Uygulamada aşağıdaki ve benzer senaryolardan elde edilen sonuçlar ekranda
gösterilmelidir:
• Senaryo 1: Ürün (Product) sütununda %60 ve üzeri benzer olan kayıtları
ekranda gösteriniz.
• Senaryo 2: Aynı ürünler (Product) için % 70 ve üzeri benzerlikteki konuları
(Issue) içeren Şirket (Company) isimlerini ekranda gösteriniz.
• Senaryo 3: ‘Complaint Id’ = 3198084 olan şikayet kaydı için % 50 ve üzeri
benzerlikteki konuları (issue) içeren kayıtları ekranda gösteriniz.
• Senaryo 4: 5 Thread ile Konular(Issue) sütununda %80 ve üzeri benzer olan
kayıtları ekranda gösteriniz

DÜZENLENMİŞ VERİ SETİNİN SON HALİ:

![image](https://user-images.githubusercontent.com/115660565/228302015-f1dc5033-cad2-4781-bccd-5c13f54cb5df.png)

ARAYÜZ FOTOĞRAFI:
![image](https://user-images.githubusercontent.com/115660565/228302134-049c8649-cc28-4f07-9327-5648d10c8a65.png)


AKIŞ ŞEMASI:

![image](https://user-images.githubusercontent.com/115660565/228302226-c6ac0d4f-7f73-4182-8c84-4ff35a8fbf66.png)



