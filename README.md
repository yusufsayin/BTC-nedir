#  Bitcoin aslında nedir?

Özel anahtarı aşağıdaki sayılar arasında her hangi biri olan bir cüzdan adresi ile birbirleri arasından BTC transferi yapan bir ağdır.


0000000000000000000000000000000000000000000000000000000000000001
fffffffffffffffffffffffffffffffebaaedce6af48a03bbfd25e8cd0364140

#  Bu sayıların özelliği nedir?
2^^0 ile 2^^256 - 2^^32 - 977 dir. Satoshi bu sayıları neden seçtiği konusunda net bir cevap yoktur. 

# Bu kadar cüzdan olduğu belli ise deneme ile bunlar tespit edilemez mi ?
Evet yeteri kadar gücün ve zamanın(!) varsa olabilir. Ancak gerçeklerle yüzleşmeye başladığında aslında o kadar kolay olmadığını iliklerine kadar hissedeceksin.

# Özel anahtar ne işe yarıyor? BTC adresi nereden geliyor?

Bir tane private key seçmek için genel kullanıcılara Tohum(Seed) dediğimiz 12-24 tane kelime verilir. Bu kelimeler işlemlerden geçirildikten sonra elde edilen özel anahtar ile işlem yapılır. 

Mesela bir cüzdan oluşturalım. Kelimlerimiz (ingilizce): barrel card promote valley pause purchase innocent hood asthma coral noise badge

Özel Anahtarımız : bed50ff13a26bf1c21dc99b232425fcb933600478e4dad5d83ae21ade919be41 (64 karakterdir)

Özel anahtar ile bitcoin adresimizi hesaplayalım,
# Sıkıştırılmamış Genel Anahtar (Public Key)
1. adım Genel/Açık Anahtarımızı (Public Key) hesaplayalım: 041e6972c9ec060a506c8f0bc12608d0fa97da88d83e38b453ab61c9d9863ec2d51b1a96e6c67c8691013ac70ba4cca8138c6abc57e67ed7780523be7a7ebe44bc (130 karakterdir)

Burada 04 sayısı her zaman bulunur.

x Koordinatı => 1e6972c9ec060a506c8f0bc12608d0fa97da88d83e38b453ab61c9d9863ec2d5

y Koordinatı => 1b1a96e6c67c8691013ac70ba4cca8138c6abc57e67ed7780523be7a7ebe44bc

# Sıkıştırılmış Genel Anahtar nedir?
Zamanla kullanıcılar aslında X koordinatının kendini tekrar ettiğini farkettiler. 

**0000000000000000000000000000000000000000000000000000000000000001** özel anahtarının X koordinatı 79be667ef9dcbbac55a06295ce870b07029bfcdb2dce28d959f2815b16f81798


**fffffffffffffffffffffffffffffffebaaedce6af48a03bbfd25e8cd0364140** özel anahtarının X koordinatı 79be667ef9dcbbac55a06295ce870b07029bfcdb2dce28d959f2815b16f81798 dır.

Y koordinatları ise farklıdır.

Hal böyle olunca Sıkıştırılmış adres diye bişey çıktı. X koordinatının başına 02 ve 03 getirerek daha kısa ve daha küçük bir sayı ile işlem yapılabildiğini keşfettiler.

**0279be667ef9dcbbac55a06295ce870b07029bfcdb2dce28d959f2815b16f81798** 
**0379be667ef9dcbbac55a06295ce870b07029bfcdb2dce28d959f2815b16f81798**

Evet bunlar ortada bir yerde buluşuyorlar.

**"7fffffffffffffffffffffffffffffff5d576e7357a4501ddfe92f46681b20a0"**

**"7fffffffffffffffffffffffffffffff5d576e7357a4501ddfe92f46681b20a1"** özel anahtarlarının X koordinatları yine aynı ancak Y koordinatları farklı.

