# BlockzincirNotlar-
Linux Yaz Kampı Blokzincir Notları

https://medium.com/@coskunnuresma/blokzincir-teknolojileri-ders-notlar%C4%B1m-lkd-linux-yaz-kamp%C4%B1-2019-dc43556ee816

I. Kriptolojiye Giriş
Hash Fonksiyonu: Uzun girdileri matematiksel fonksiyonlarla sabit uzunlukta eşsiz bir değere çevirme işlemidir.
 i.Avantajları: Veri girişinde değişiklik olduğunda hash fonksiyonu değişeceği için, girilen veride değişiklik yapılıp yapılmadığını kontrol etmek için kullanabiliriz.
 ii.Veri güvenliğini sağlar.
 iii.Verilerin sınıflandırılmasında kullanılır.
 iv.MD5, SHA1, HAVAL buna örnek verilebilir.
Sezar Şifreleme Algoritması: Açık metindeki harfler kendinden 3 harf sonraki harf ile şifrelenir.

Sezar Şifreleme Algoritmasının Çalışma Prensibi
3. RSA Şifreleme Algoritması: RSA’e atak yapmak mümkün. RSA private anahtarı yazılım veya donanım içerisinde tutabilir.
i. Analytics Attack: Saldırı alanını küçültüp, mantıksal atak yapar.
ii. Implementation Attack
iii. Side-Channel Attack
iv. Fault Injection Attack
v. Matematiksel Saldırı
vi. Protokol Saldırı
vii. Vektörel Saldırı
viii. Brute-Force Attack: Elde herhangi bir veri olmadan yapılan saldırıdır. Deneme yanılma yoluyla işlemektedir. Anahtara sağdan ve soldan saldırır (paralel).


RSA Şifreleme Algoritmasının Çalışma Prensibi
4. AES Şifreleme Algoritması: AES üç blok şifre içerir.

i. AES-128, bir mesaj bloğunu şifrelemek ve şifresini çözmek için 128 bitlik bir anahtar uzunluğu kullanır.

ii. AES-192, bir mesaj bloğunu şifrelemek ve şifresini çözmek için 192 bitlik bir anahtar uzunluğu kullanır.

iii. AES-256, bir mesaj bloğunu şifrelemek ve şifresini çözmek için 256 bitlik bir anahtar uzunluğu kullanır.

Her şifre, sırasıyla 128, 192 ve 256 bitlik kriptografik anahtarları kullanarak 128 bitlik bloklardaki verileri şifreler ve şifresini çözer.

Gizli anahtar olarak da bilinen simetrik şifreler, şifreleme ve şifre çözme için aynı anahtarı kullanır. Gönderici ve alıcı aynı gizli anahtarı bilmeli ve kullanmalıdır.


AES Şifreleme Algoritmasının Çalışma Prensibi
5. Hibrit Şifreleme Algoritması: Mesajı simetrik şifreleme algoritması şifreler. Gizli anahtarı asimetrik şifreleme algoritması şifreleyerek alıcıya ulaştırır.

6. Dijital İmza (5070 sayılı kanunda yer alıyor.): Dijital imzada mesaj hash fonksiyonu ile tutulmaktadır. Mesaj değiştiğinde imza da değişmektedir.

7. Block Şifreleme: Bu yöntemde, açık metin belirli uzunluklarda bloklara bölünür. Bölünen bloklar ayrı ayrı şifrelenir. Şifreli metin bu blokların dizilimi ile elde edilecektir.

a. Örn: Şifrelenecek metin “Ali baba ve kırk haramiler”
1)Aliba 2)Bavek 3)Irkha 4)Ramil 5)Er
Bu beş blok ayrı ayrı şifrelendikten sonra elde edilen veriler bir araya
getirilerek şifreli veri elde edilir.

8. Stream Şifreleme: Şifreleme birimindeki işlem bir önceki şifreleme işlemine bağlıdır. Her harfin şifrelenmesi sırasında bir önceki şifrelemeden çıkan bilgi anahtar olarak kullanılabilir.


*PRNG: Sözde Rastsal Sayı Üreteci
*CSPRNG: Kriptografik Olarak Sözde Rastsal Sayı Üreteci

9. OTP(One Time Pad): Bankaların yolladığı tek seferlik parolalar örnek verilebilir.
a. Dezavantajı: Pratik olmaması.


10. Kriptografik Hash Fonsiyonu:
a. 1 girişin (input) 1 çıkışı (output) vardır.
b. Farklı 2 input aynı outputu vermez.
c. Hash fonksiyonu geri döndürülemez, orijinal metine ulaşılamaz.
d. Bir harfin değişmesi tüm hash fonksiyonunu değiştirir.

11. Peer To Peer (P2P): Hem istemci hem server gibi davranabilen ağ protokolü.
a. Ağdaki başka kişilere verinin doğruluğu sorulabilir.
b. Merkezi koordinasyona ihtiyaç yoktur.
c. Avantajları: Dağıtık bir sistem olduğu için veriler silindiğinde kaybolmaz. Erişim problemi ortadan kalkar.(merkeziyetsiz)
d. Dezavantajları: Kullanıcı olmadığı sürece anlamı kalmaz.
e. Problemler: Ağdan veriyi çektikten sonra “atak vektörler” olma ihtimali vardır. Ağda sadece veriyi çekmek isteyen kişiler de olabilir.

12. Zero Knowledge Proof: Bir bilgiyi bildiğimi, karşı tarafa bu bilgiyi vermeden nasıl ispat edebilirim? Sorusunun cevabını arar.
a. 1.taraf provers
b. 2.taraf verifier: mesajın doğruluğunu onaylar.
c. Peki verifier güvenilir değilse?
i. ZKP for 3 coloring: Bu yöntemde Alice bildiği bilgiyi Bob’a graphdaki seçilen gizli nodeları açıp rengini göstererek kanıtlayabilir.

*Fiat Shamir Heuristic (Non interactive): Kriptografide etkileşimli bir bilgi kanıtı almak ve buna dayanarak dijital imza oluşturmak için kullanılan bir tekniktir.
*ZeroCoin Protokolü
*ZeroCash ZK-SNARKS Protokolü

13. Graph Isomorphism: Graph teoriye göre iki şekil birbirinden farklı çizilmiş fakat işlev ve değer olarak aynı olabilir.


Schnorr Identification Protocol: Dijital imzaya göre daha güvenli bir protokoldür. İmzaya benziyor fakat bunu zkp ile yapar.

ZKP ile blockchain nasıl kullanılır?
a. Veri miktarı, kime gideceği vb. bilgiler gizli tutulabilir.

Distributed Ledger: Kayıtların dağıtık tutulması.
*Single Point of Failure: Tek bir yerde tutulan verinin bozulması.

P2P+Distributed Ledger+Hash Fonsiyonu Kullanımı:
a. P2P ile kullanıcı birçok ağa erişebilir.
b. Distributed Ledger ile P2P ağına veriler dağıtık kayıt edilebilir.
c. Hash fonksiyonu ile bu veriler hashlenir ve değişiklik olduğunda fark edilmesi sağlanır.

P2P Kullanımına Örnek ‘Karayolları’:
a. Devletten para almak için, şirketlerin yol bakımında yapılan değişiklikleri ve tedarikçiden satın aldığı malzemeleri sisteme girmesi gerekir.
b. Şirket veri girmezse yol bakımı yapılmadığı için veya tedarikçiden eksik ürün alınması durumunda devlete tazminat ödemesi gerekir.

II. Blokzincire Giriş
Blokzincirde bloklar birbirine bağlı veri taşır. Bu veriler hash ile paketlenir, verinin değişmezliği korunur.


Smart Contract: Sözleşmeyi kullanan tüm tarafların kabul ettiği koşulları belirtir. Gerekli şartlar sağlandığında bazı eylemler yapılır.
Mining Node: İşlemlerin gerçekleşmesini sağlayan bilgisayarlardır.
Para:
a. Bilinirlik
b. Bölünebilme
c. Taşınabilirlik
d. Güven mekanizması (sahteliğe karşı)
e. Üretim politikası
f. Paranın arkasındaki otorite (paranın değeri)
Wallet: Bitcoinleri yöneten birim. *Ne kadar bitcoin olduğunu göstermeli. Gizli anahtarı tutar.

*Transaction fee miktarı fazlaysa, işlem hızlı yapılır.
*Wallet rastgele bir kümeden transfer edilecek olan miktarı çıkarır. Geriye kalan parayı (10 btc — 7 btc=3 btc) parayı gönderen walleta yatırır.

a. Cold Wallet: Offline, internet bağlantısı yok.
b. Hot Wallet: İnternete bağlı cihazlarda saklanan anlık transactionları saklamaya yarar. Online olduğu için hack riski var.

*ÖDÜL: Her miner işlediği bloğun transaction fee’sini ve bulduğu bloğun ödülünü 12.5 BTC alır.
*Miner bloka kendi seçtiği (muhtemelen transaction fee en yüksek olanları) gelen transactionları yazar. Eğer blok kazılmadan/ bulunmadan transaction yapıldıysa kullanıcı bir sonraki bloğun oluşmasını bekler. Bir sonraki blok oluşana kadar transactionlar memory pool’da bekler.

Double Spending: Aynı parayı iki farklı kişiyle paylaşma. Çifte harcama. Tek dijital jetonu birden fazla harcama.

Difficulty: 2016 blokta bir zorluk hesaplanır. Blok 2 haftadan önce bulundu ise zorlaşır sonra bulundu ise kolaylaşır.
a. Ağın zorluğu her 2016 blokta bir değişir.
b. Sıfırın artışı ya da azalışı zorluğu belirler. Zorluk derecesini “n” adet “0”ile başlaması belirliyor. 2n zorluk derecesine sahiptir.
i. 0000005A4….  Miner’ler random bu değerleri bulmaya çalışır.
ii. 0007B8…… Miner’ler random bu değerleri bulmaya çalışır.

III. Bitcoin
Bitcoin (Limit 21 Milyon)
a. Her 10 dakikada 1 blok = 12.5 BTC

b. Her saatte 6 blok.

c. Her günde 144 blok =180 BTC

d. Her 210.000 blokta bir %50 düşüyor.

e. 50.(1+1/2+1/4+…)

f. 50.2=100, 210.000*100=21 milyon adet

2. Mining
a. %51 Saldırısı: Bu saldırıyı yapabilmek için sistemde %50 güce sahip olmak gerekir.
i. Bu saldırıyla yapılan (belli public key ile) işlemler geçersiz sayılabilir.
ii. Sahte hash üretilebilir.
iii. Double Spending yapılabilir.
b. 1/3 Node Saldırısı (BFT: Bizans Fault Tolerans)
i. Matematiksel olarak çalışır.
ii. Hiçbir zaman yapılamadı.
c. Peer Authentication: DNS sunucusu üzerinden direkt ip adresini çekmeyi sağlıyor. Seed elde ediyor. IP adresini isteyebilir veya DNS ile direkt çekilir.
i. Trusted Ip: Minerların ip adresini bulmamıza yardımcı bir authentication.
d. Selfish Mining: Selfish mining ihtimaline karşı transfer yapıldıktan sonra 7 blok beklenmeli. Böylece işlemin doğruluğu teyit edilebilir.


e. POW Enerji Tüketimi
f. Pool Mining Mantığı
g. Wallet Fishing: Web sitelerde satışı yapılan walletlerın private key değeri bilindiği için kullanıcıların bitcoinlerine ulaşılabilmektedir.

3. Blok: Toplam 1 MB’dır.


4. Merkle Tree: Blokta değişiklik olduğunda diğer bloklar kırılır. Bloğun hashini alır.


*Genesis bloktaki bir veri değiştirildiğinde bağlı olan tüm blokların tekrar mine edilmesi gerekir.
*Miner nonce değerini bulursa bloğu işlemeye hak kazanır.


IV. Ethereum
Ethereum ağında kurallar bir kere yazıldıktan sonra değiştirilemez, geri alınamaz.
a. Her bilgisayarda contract ve ledger tutulur.
b. Kodlar yazılıp çalıştırıldıktan sonra değiştirilemez.
c. Contracta ether yollanabilir.
d. Contract zamanla sınırlandırılabilir (Çalışmaya başladıktan 1 ay sonra durdur gibi.).
e. Gas fee = transaction fee
D.A.O (decentralized autonomous organization)
D.A.P.P
1. Smart Contract: Ethereum Virtual Machine’de çalışır ve işlem başına GAS alınır.
2. Gas: Gas için ödenen para miktarı minerlara gider.
a. 1 ETH=97 Milyon Gas
b. Contract yazıldıktan sonra ether ile gas alınır.Contract öyle yayınlanır.?
3. POS (Proof Of Stake): Ağda ne kadar zenginsen o kadar güçlüsün. Mining yok, genesis blokta tüm üretim yapılır.
a. Küçük işlemler POS ile, büyük işlemler POW ile yapılır.
b. Ethereum POW kullanırken çok enerji harcadığı için POS’a geçmiştir.
4. Integrated Oracle: Smart contract sonunda işi yapan veya işi yaptıran taraflardan biri işin yapılmadığını söylerse integrated oracle işin yapılıp yapılmadığını tespit eder.


ERC-20 ve EIP-20 Token Standard
5. Master Node(POSE): Block işleyen VPS’lerdir.
a. Dash coin de kullanılıyor.
b. 1 Master node=1000 Dash
c. Saniyede 1 blok oluşturuluyor.
d. Master node sayısı miner sayısını verir.
e. Fee:
i. %40 Miner
ii. %40 D.A.O
iii. %20 Dash Core
f. Master node’ların her biri full node’dur.
*Full Node: Tüm defteri (ledger) sürekli olarak içinde bulunduran node’lardır.


6. Dash Algoritması:
a. Hash fonksiyonu gibi girdi aynı olsa da çıktı farklıdır.
b. İşlemi yapacak master node random seçilir.
c. 1–3 saniyede bir block oluşturulur.
*Tek başına miner olmak için full node olmak gerekir.

Node Çeşitleri

a. Light Nodes:
i. Tek başına mining yapamaz.
ii. Mining pool’larda olur.
iii. Mining pool’daki işlemlerin hızlanması için kullanılır. Cache gibi.
iv. Memory pool’dan veri çekerken oluşan 1–2 saniyelik gecikmeyi engeller.
v. Yapılan son işlemi tutar.(Son 300–400 transaction tutar.)
b. Full Nodes:
c. Pruned Nodes:
i. Mining yapamaz.
ii. İşlenen bütün nodeları kopyalar.
iii. Depolama kalmadığında eski transactionları silip (veri) sadece headerı saklar.
iv. Zincirin kırılmadığının garantisini sağlar.

d. Archival Nodes:
i. Mining yapabilir.
ii. Tüm transactionları saklar.
iii. Full Node’dur.
iv. Master Node: Bir archival node’dur.
v. Mining Node:
1) Pool’u yöneten kişi minig node’dur.
2) Full node*cpu+gpu gücü vardır.
vi. Staking Node: POS’daki staking üzerinden mining yapan nodelara staking node denir.
vii. Authority Node:
1) Network’e girecek kişileri authority node belirler.
2) Merkez tarafından node olup olmayacağınız belirlenir.
3) Network’de en az 1 kişi memory pool’u tutmak zorundadır.
4) Coin ve fee yoktur.

7. Hibrit Network/ Off Chain: Ether networkünde public key ile dahil edilebilen iç/özel network kurulur. İç networkde işlemler (smart contract) yapıldıktan sonra ortaya çıkan ödemeler Ether bloğuna tek bir transaction olarak kayıt edilir. ÖRN: kumarhaneler.
a. Dış networkte para transferi yapıldığı gözükse de ne için para transferi yapıldığı bilinemez.

8. IOTA: İot cihazlar arası haberleşmeyi sağlamak amacı ile neighboard’lar arasında iletilir. İletildikten sonra veri silinir. Fee yanar.

9. AVA Project: Herkes “n” adet node’dan sorumlu (genelde 5 adet). Her n küme kendi etrafına bakarak 17 turda doğru karara varabiliyor. 1.7 saniyede bir blok herkes tarafından kontrol sonrası aktif edilir. Mining yok.

Bitcoin Wallet’ı Oluşturmak İçin:


Neden Hyperledger:
a. Kimlik doğrulaması
b. Veri gizliliği
c. Modüler mimari
d. Dil seçenekleri
e. Ücretsiz
f. Hız

Hyperledger Fabric vs Hyperledger Composer: Composer Fabric’in kolay kullanımı için fakat opsiyoneldir ama iyi bir başlangıç için önerilmektedir.
