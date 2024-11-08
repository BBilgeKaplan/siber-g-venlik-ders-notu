# IP Adresi Nedir?

IP adresleri (Internet Protocol Address), internete veya başka bir ağa bağlı her cihazın tanımlanmasını sağlayan benzersiz numaralardır. IP adresleri iki ana kategoriye ayrılır: Public ve Private.

## Public IP Adresi

**Public IP adresi**, internet servis sağlayıcınız (ISP) tarafından atanır ve internete erişiminizi sağlar. Bu adresler, dünya genelinde benzersizdir ve internet üzerindeki diğer cihazlar tarafından görülebilir. Örneğin, bir web sitesine eriştiğinizde, bu siteye sizin public IP adresinizden ulaşırsınız.

### Özellikleri:
- İnternet üzerinde benzersizdir.
- ISP tarafından atanır.
- Herkes tarafından görülebilir.

## Private IP Adresi

**Private IP adresi**, ev veya işyeri gibi özel ağlar içinde kullanılır ve bu ağdaki cihazlar arasında iletişim sağlar. Bu adresler, aynı ağ dışındaki cihazlar tarafından görülemez. Genellikle router (yönlendirici), bu private IP adreslerini cihazlara otomatik olarak atar.

### Özellikleri:
- Yerel ağlarda kullanılır.
- İnternet üzerinde benzersiz değildir.
- Yönlendirici tarafından atanır.

Örneğin, bir ev ağı düşünün. Router, ev içindeki cihazlara private IP adresleri atar (örneğin, 192.168.1.2). Bu cihazlar, internete bağlanmak için router üzerinden public IP adresini kullanır.

![image](https://github.com/user-attachments/assets/77cd4e04-0cd3-49eb-9578-de6190d8ed15)  

![image](https://github.com/user-attachments/assets/b86ecc1d-41af-4103-8585-012817c1a434)  

![image](https://github.com/user-attachments/assets/c74f45b0-9fa4-438d-861c-ae8d135f8f99)  


# MAC Adresi
MAC (Media Access Control) adresi, bir ağ cihazına (örneğin, bilgisayar, telefon, modem gibi) üretici tarafından atanan benzersiz bir kimlik numarasıdır. Her cihazın kendine özgü bir MAC adresi vardır ve bu adres, cihazların yerel ağdaki (LAN) iletişiminde kullanılır. MAC adresi, ağ kartı seviyesinde çalışır ve ağ üzerinde hangi cihazın veri gönderip aldığını tanımlar. Bu adres, 48 bit uzunluğunda olup, genellikle altı adet ikili gruptan oluşan onaltılık sayı (örn. 00:1A:2B:3C:4D:5E) biçiminde yazılır.

## MAC Adresi Saldırıları
MAC adresi, yerel ağlarda cihazları tanımlamak için kullanılır, bu yüzden saldırganlar için cazip bir hedef olabilir. İşte MAC adreslerine yönelik bazı yaygın saldırılar:

- MAC Spoofing (MAC Sahteciliği): Saldırganın kendi cihazındaki MAC adresini, ağda güvenilir bir cihazın MAC adresiyle değiştirerek kimliğini gizlemesidir. Böylece ağda başka bir cihaz gibi davranarak erişim sağlayabilir. Bu, özellikle kimlik doğrulamanın MAC adresine göre yapıldığı ağlarda saldırganın yetkisiz erişim sağlamasına olanak tanır.

- MAC Flooding (MAC Taşkını): Bu saldırıda saldırgan, bir switch'e aynı anda çok sayıda sahte MAC adresi gönderir. Switch’in MAC adres tablosu dolarak aşırı yüklenir ve switch gelen verileri doğru cihaza yönlendiremez hale gelir. Sonuç olarak switch, tüm veriyi ağdaki bütün portlara göndermeye başlar ve saldırganın ağ trafiğini izlemesini sağlar.

- Man-in-the-Middle (MitM) Saldırıları: Bu tür saldırılarda saldırgan, hedef cihaz ile diğer cihazlar arasındaki trafiği izlemek ve değiştirmek için MAC spoofing veya diğer yöntemleri kullanarak cihazların arasında yer alır. Bu şekilde, veriler saldırganın cihazı üzerinden geçerken dinlenebilir veya değiştirilebilir.  

# Firewall (Güvenlik Duvarı)
Firewall, bir ağın güvenliğini sağlamak için gelen ve giden trafiği kontrol eden bir güvenlik cihazıdır. Belirli kurallar veya filtrelere göre trafiği engelleyebilir veya geçirebilir. Ağ içindeki zararlı trafiği veya istenmeyen erişimleri engellemek için kritik bir güvenlik unsurudur. Yazılım veya donanım tabanlı olabilir.  
Portlar kullanılır. Servislere erişim ayarlanır.  
Genelde izin ver (allow) veya yasakla (deny) prensibine göre çalışır.  
Günlük Kayıtları (Logging): Tüm aktiviteleri kaydederek izleme ve analiz yapmaya olanak tanır.

# Hub (Dağıtıcı)
Hub, bir ağda birden fazla cihazın birbirine bağlanmasını sağlayan basit bir ağ cihazıdır. Temelde veriyi bir cihazdan alır ve bu veriyi ağdaki tüm diğer cihazlara iletir.  
OSI de fiziksel katmanda yer alır.  

### Hub vs. Switch
- Verimlilik: Hub, veriyi tüm cihazlara iletirken, switch veriyi yalnızca hedef cihaza yönlendirir. Bu da switch'i daha verimli kılar.  
- Çakışma: Hub'da çakışmalar daha sık görülürken, switch bu çakışmaları önler.  
- Fiyat: Hub'lar genellikle daha ucuzdur ve basit ağlarda kullanılır.  

Hub, temel ağ bağlantıları sağlasa da, modern ağlarda switch'ler daha yaygın olarak kullanılır çünkü daha verimli ve güvenilirdir.


# Switch Nedir?
Switch, bir yerel alan ağı (LAN) içinde cihazları (bilgisayarlar, yazıcılar, sunucular vb.) birbirine bağlayan ağ cihazıdır. Switch, ağın farklı cihazları arasında veri paketlerini yönlendirmek ve iletmek için kullanılır. Bu sayede ağ içindeki cihazlar arasında hızlı ve güvenli iletişim sağlanır.

Switch, daha önce kullanılan hub cihazlarına göre daha akıllı bir cihazdır. Hub'lar, gelen veriyi tüm portlara ileterek bant genişliğini verimsiz kullanırken, switch'ler veriyi sadece hedef cihaza yönlendirir. Bu sayede daha verimli bir ağ trafiği sağlanır.  

![image](https://github.com/user-attachments/assets/3c9418fb-6a60-455c-97eb-96d17fad0d77)  

### Switch'in Çalışma Mantığı
Switch'ler, OSI modelinin veri bağlantı (data link) katmanında (Layer 2) çalışır.  
Verilerin MAC adreslerine göre yönlendirilmesini sağlar.  
Switch'in çalışma prensipleri:

#### MAC Adres Tablosu Oluşturma
- Switch, ağdaki cihazların MAC adreslerini öğrenmek ve depolamak için MAC adres tablosu oluşturur. Bu tablo, switch'e hangi porttan hangi MAC adresine sahip cihazın bağlı olduğunu gösterir.
- Switch, bir veri paketi ilk kez geldiğinde kaynak MAC adresini kaydeder ve bu MAC adresinin hangi porttan geldiğini tabloya ekler.
- Eğer hedef MAC adresi bu tabloda varsa, switch bu port üzerinden veriyi doğrudan hedef cihaza iletir. Tabloda yoksa, veri paketi tüm portlara (flooding) iletilir, bu sayede hedef cihaz bulunur ve tabloya kaydedilir.

#### Çerçeve Yönlendirme
- Switch'e gelen veri paketleri, çerçeve (frame) olarak adlandırılır. Switch, bu çerçeveleri kaynağından hedefe yönlendirir.
- Veriyi alır ve hedef MAC adresine göre ilgili porttan gönderir. Bu, trafiğin sadece ilgili cihazlar arasında iletilmesini sağlar ve ağın genel performansını artırır.
- Switch, yalnızca Layer 2 değil, Layer 3 (Ağ katmanı) özellikleri de destekleyebilir. Bu durumda switch, router gibi IP yönlendirmesi de yapabilir ve buna katman 3 switch denir.

#### Tam ve Yarım Çift Yönlü İletim (Full/Half Duplex)
- Tam çift yönlü (Full Duplex) iletişimde, switch hem veri alabilir hem de veri gönderebilir. Bu, ağ performansını artırır çünkü veri transferi çift yönlü ve aynı anda gerçekleşebilir.
- Yarım çift yönlü (Half Duplex) iletişimde ise veri aynı anda sadece bir yönde gider; yani veri gönderilirken alınamaz. Bu tür iletişim, daha eski cihazlarda ve hub'larda yaygındır.

### Switch Çeşitleri
Switch'ler, farklı kullanım alanlarına ve özelliklerine göre çeşitli türlerde gelir:

#### Unmanaged (Yönetilmeyen) Switch
- Kullanıcı müdahalesi gerektirmeyen basit switch'lerdir. Genellikle tak-çalıştır özelliklidir. Küçük ofislerde veya ev ağlarında kullanılır.
- Yönetim ve konfigürasyon seçenekleri sınırlıdır.

#### Managed (Yönetilen) Switch
- Ağ yöneticisinin, switch'i yapılandırmasına, ağ trafiğini izlemeye ve yönetmeye olanak tanır. Büyük ve karmaşık ağlarda tercih edilir.
- VLAN oluşturma, QoS (Quality of Service) ayarları, port güvenliği gibi özellikleri destekler.
- CLI (Komut Satırı Arayüzü) veya GUI (Grafik Kullanıcı Arayüzü) aracılığıyla yapılandırılabilir.

#### Layer 3 Switch (Katman 3 Switch)
- Yönlendirme (routing) işlevlerini de yerine getirebilen gelişmiş switch'lerdir. Bu switch'ler, hem Layer 2 çerçeve yönlendirmesi hem de Layer 3 IP yönlendirmesi yapabilir.
- Genellikle büyük kurumsal ağlarda kullanılır, çünkü router'lardan daha hızlı veri işleme yeteneğine sahiptir ve ağın performansını artırır.

### Switch'in Temel Özellikleri ve Kullanım Alanları
- **Port Sayısı**: Switch'ler genellikle 8, 16, 24 veya 48 portlu olabilir. Kullanım amacına göre port sayısı seçilir.
- **VLAN Desteği**: Bir switch'te sanal yerel alan ağları (VLAN) oluşturulabilir. Bu, büyük ağların farklı segmentlere bölünmesini sağlar ve ağ trafiğini düzenler.
- **PoE (Power over Ethernet)**: PoE özellikli switch'ler, bağlı cihazlara (örneğin, IP telefonlar, kablosuz erişim noktaları, güvenlik kameraları) veri ile birlikte elektrik gücü de iletebilir.
- **QoS (Quality of Service)**: Trafik önceliklendirmesi sağlar, böylece ses ve video gibi zaman hassasiyeti olan uygulamalara öncelik verilir.

### Switch Kullanımının Avantajları
- **Yüksek Performans**: Veri trafiği hedef cihazlara yönlendirildiği için ağın genel bant genişliği daha verimli kullanılır.
- **Daha Az Çakışma**: Switch'ler, çerçeveleri doğrudan hedef cihaza yönlendirdiği için hub'lara kıyasla çakışmaların önüne geçer ve daha hızlı veri iletişimi sağlar.
- **Güvenlik**: Yönetilen switch'lerde port güvenliği gibi gelişmiş güvenlik önlemleri uygulanabilir. VLAN'lar kullanılarak ağ segmentasyonu ve trafik kontrolü sağlanır.

# Router Nedir?

Router, iki veya daha fazla bilgisayar ağı arasında veri paketlerini yönlendiren bir ağ cihazıdır. Router'lar, yerel ağ (LAN) ile geniş alan ağı (WAN) arasında köprü kurar ve internet trafiğini yönetir.  
IP adreslerini kullanır. OSI'de 3. katmandadır.

## Router'ın İşlevleri

1. **Veri Yönlendirme**: Router, IP adreslerini kullanarak veri paketlerini doğru hedefe yönlendirir.
2. **Ağ Bağlantısı**: Farklı ağları birbirine bağlar ve veri alışverişini sağlar.
3. **Güvenlik**: Güvenlik duvarı özellikleri sayesinde ağa yetkisiz erişimi engeller.
4. **NAT (Ağ Adresi Çevirisi)**: Private IP adreslerini public IP adreslerine çevirerek, internete erişimi sağlar.

## Router'ın Çalışma Prensibi

1. **Veri Paketlerini Alma**: Router, bir cihazdan gelen veri paketini alır.
2. **IP Yönlendirme**: IP adresini kontrol ederek, paketin hedef IP adresine göre uygun ağ yolunu belirler.
3. **Veri İletimi**: Paketi, hedef IP adresine en kısa ve en hızlı yoldan iletir.
4. **Adres Çevirisi (NAT)**: Private IP adreslerini public IP adreslerine çevirir, böylece cihazlar internete bağlanabilir.

## Router'ın Avantajları

- **Güvenlik**: NAT ve güvenlik duvarı özellikleri ile ağ güvenliğini sağlar.
- **Bağlantı Çeşitliliği**: Hem kablolu hem de kablosuz bağlantı imkanı sunar.
- **Verimli Veri Yönlendirme**: Veri paketlerini en uygun yollar üzerinden yönlendirerek ağ performansını artırır.

# Gateway
iki farklı ağ arasındaki trafiği yönlendiren ve çeviren bir ağ cihazıdır. İki farklı ağ arasında veri iletişimini sağlar ve genellikle yerel ağ (LAN) ile geniş alan ağı (WAN) arasında kullanılır.
Genelde routerlar üzerinden tanımlanır. Farklı protokol kullanan ağlarda iki yönlü protokol dönüşümü yaparak bağlantı yapılmasını sağlar.  
OSI'de tüm katmanları içerir.

# Alt Ağlara Bölme (Subnetting) Nedir?

Alt ağlara bölme (subnetting), büyük bir IP ağıyı daha küçük, daha yönetilebilir alt ağlara bölme işlemidir.  
Bu, ağın verimli kullanımını sağlar ve ağ trafiğini yönetmeyi kolaylaştırır.

## Nerede Kullanılır?

- Büyük şirket ağlarında
- Veri merkezlerinde
- İnternet Servis Sağlayıcılarında (ISP)
- Birden fazla bölgeye dağılmış ofislerde

## Ne İşe Yarar?

- Ağ trafiğini optimize eder.
- Ağ güvenliğini artırır.
- Ağ yönetimini kolaylaştırır.
- IP adreslerinin verimli kullanımını sağlar.
- Temel Network Tanımları:

**IP Adresi**: Bir cihazın ağa bağlandığında aldığı benzersiz adres.  
**Alt Ağ Maskesi (Subnet Mask)**: Hangi IP adreslerinin aynı alt ağda olduğunu belirler.  
**Network ID (Ağ Adresi)**: Network ID, bir alt ağdaki cihazların aynı ağda olduğunu belirtmek için kullanılan adres kısmıdır. IP adresi ve alt ağ maskesinin AND işlemi ile bulunur.  

Örneğin:  

IP Adresi: 192.168.1.10   
Alt Ağ Maskesi: 255.255.255.0  

AND işlemi:  
192.168.1.10 = 11000000.10101000.00000001.00001010  
255.255.255.0 = 11111111.11111111.11111111.00000000  
— — — — — — — — — — — — — — — — — — — — — — -  
192.168.1.0 = 11000000.10101000.00000001.00000000

## Alt Ağ Maskesi (Subnet Mask) Nedir?

Alt ağ maskesi, bir IP adresinin hangi kısmının ağ adresi ve hangi kısmının cihaz (host) adresi olduğunu belirler.

# DNS (Domain Name System) Nedir?
DNS (Domain Name System), internet üzerindeki alan adlarını (domain names) IP adreslerine çeviren bir sistemdir. İnsanlar web sitelerine alan adları (örneğin, www.example.com) üzerinden erişmeyi tercih ederken, bilgisayarlar ve ağ cihazları bu alan adlarını IP adresleriyle (örneğin, 93.184.216.34) tanır ve kullanır. DNS, bu çeviriyi otomatik ve hızlı bir şekilde yaparak kullanıcıların alan adları ile web sitelerine ve diğer internet hizmetlerine erişimini sağlar.

## DNS Nasıl Çalışır?
DNS'in çalışma prensibi birkaç temel adımdan oluşur:

**1. Alan Adı Girişi ve İstemci İsteği:**

- Kullanıcı bir web tarayıcısına "www.example.com" gibi bir alan adı girdiğinde, cihaz DNS sunucusuna bir sorgu gönderir. Bu sorgu, alan adının IP adresini sormaktadır.

**2. Yerel DNS Önbelleği Kontrolü:**

- Cihaz öncelikle kendi önbelleğinde (cache) bu alan adı ile ilişkili bir IP adresi olup olmadığını kontrol eder. Eğer bulursa, DNS sunucusuna gitmeden IP adresini kullanarak bağlantı kurar.

**3. DNS Sunucusuna İstek Gönderme:**

- Cihazın önbelleğinde bilgi yoksa, sorgu yerel DNS sunucusuna (genellikle internet servis sağlayıcısının DNS sunucusu) gönderilir.

**4. DNS Çözümleme (Recursive Query):**

- Eğer yerel DNS sunucusunda da bilgi yoksa, bu sunucu daha üst seviyedeki DNS sunucularına (root DNS sunucuları) isteği ileterek IP adresini bulmaya çalışır.
- Root DNS sunucuları, alan adı uzantılarını (.com, .org, .net vb.) yöneten üst DNS sunucularına yönlendirme yapar. Örneğin, ".com" uzantısını yönetmekten sorumlu olan sunucuya istek gönderilir.
- Bu sunucu, belirli bir alan adının yetkili DNS sunucusuna yönlendirme yapar.

**5. Yetkili DNS Sunucusuna İletme ve Yanıt Alma:**

- Alan adı ile ilişkili IP adresini içeren yetkili DNS sunucusu, yerel DNS sunucusuna IP adresini gönderir.
- Yerel DNS sunucusu, aldığı yanıtı kullanıcıya iletir ve önbelleğine kaydeder.

**6. Bağlantı Kurma:**

- Kullanıcı cihazı, aldığı IP adresini kullanarak web sitesine bağlantıyı kurar.

## DNS Güvenliği ve Sorunlar
DNS, internetin önemli bir bileşeni olduğundan saldırganların da hedefi olabilir:  

**DNS Spoofing (DNS Zehirleme):** Sahte DNS yanıtları göndererek kullanıcıların sahte web sitelerine yönlendirilmesini sağlar. Bu saldırılar genellikle kullanıcıların hassas bilgilerini çalmak için yapılır.  

**DDoS Saldırıları:** DNS sunucularını hedef alan Dağıtılmış Hizmet Engelleme (DDoS) saldırıları, sunucuları aşırı yükleyerek çalışmaz hale getirebilir.  

**DNSSEC (DNS Security Extensions):** DNS sorgularının doğruluğunu ve bütünlüğünü korumak için eklenen bir güvenlik özelliğidir. DNSSEC, DNS kayıtlarının kimlik doğrulamasını yapar ve DNS zehirleme gibi saldırıları engellemeye yardımcı olur.

## DNS Spoofing Nedir?
DNS spoofing, kullanıcıların meşru bir web sitesine gitmek istediklerinde yanlış bir IP adresine yönlendirilmesini sağlayan bir siber saldırı türüdür. Bu saldırı, DNS kayıtlarının manipüle edilmesiyle kullanıcıların sahte web sitelerine yönlendirilmesine yol açar. Genellikle bu sahte siteler, kullanıcıların kişisel bilgilerini (şifreler, kredi kartı numaraları vb.) çalmak veya kötü amaçlı yazılım yaymak amacıyla kullanılır.

### DNS Spoofing Nasıl Çalışır?
DNS spoofing'in temel prensibi, DNS sorgularının sonucunu değiştirmek veya DNS sunucularını yanlış bilgi vermeye zorlamaktır. Bu saldırı birkaç farklı yolla gerçekleştirilebilir:

#### DNS Cache Poisoning (Önbellek Zehirleme):

Tanım: Bu yöntemle, DNS sunucularının önbelleğine sahte IP adresleri eklenir. DNS sunucusu, yanlış bilgiyi kullanarak kullanıcıları saldırganın kontrolündeki sahte bir web sitesine yönlendirir.
Nasıl Yapılır: Saldırgan, bir DNS sunucusuna sahte bir yanıt gönderir ve bu yanıtı sunucunun önbelleğine kaydettirir. Sonrasında, kullanıcılar bu sunucuya başvurduğunda sahte IP adresi döner ve kullanıcılar sahte siteye yönlendirilir.
Örnek: Kullanıcı "www.banka.com" sitesine gitmek istediğinde, DNS sunucusu sahte bir IP adresini döner ve kullanıcı aslında "www.sahte-banka.com" gibi bir siteye yönlendirilir.

#### Man-in-the-Middle (MitM) Saldırıları:

Tanım: MitM saldırılarında, saldırgan DNS istemcisi ve DNS sunucusu arasında durarak trafiği izler ve manipüle eder. Bu şekilde, kullanıcı DNS sunucusuna sorgu gönderdiğinde saldırgan sorguyu ele geçirir ve sahte bir yanıtla kullanıcıyı sahte bir IP adresine yönlendirir.
Nasıl Yapılır: Saldırgan, kullanıcının DNS sunucusuyla iletişimini keserek kendi sahte yanıtını gönderir. Kullanıcı, saldırganın sunduğu sahte IP adresine yönlendirilir.

#### Yerel Ağ Tabanlı DNS Spoofing:

Tanım: Saldırgan, kullanıcının bulunduğu yerel ağdaki trafiği dinleyerek DNS sorgularına sahte yanıtlar verir. Özellikle halka açık Wi-Fi ağlarında bu tür saldırılar yaygın olabilir.
Nasıl Yapılır: Saldırgan, ağa bağlı diğer cihazların DNS isteklerini yakalayarak kendi sahte yanıtını döner ve kullanıcıları kendi belirlediği sahte sitelere yönlendirir.
