<h1 align="center"> Sui Devnet Node Kurulumu </h1> 

Not: Türkçeye çevrilmiştir, alıntıdır.
![image](https://user-images.githubusercontent.com/101149671/178116806-26715fca-3ff8-43d5-ae1e-cee3926828de.png)

# Telegram kanalı: https://t.me/SuiTurkish

# Gereksinimler (minimum) (ekip tavsiyesi 8 ram):
```
2 CPU
4 RAM
50 SSD
```
Node kurduktan sonra sonda söyleyeceğim işlemleri yapmayı unutmayın!!

# Bir screen oluşturalım:
```
screen -S sui
```


# Kurulum:
```
wget -O sui.sh https://raw.githubusercontent.com/kj89/testnet_manuals/main/sui/sui.sh && chmod +x sui.sh && ./sui.sh
```

# Güncelleme: 
```
wget -qO update.sh https://raw.githubusercontent.com/kj89/testnet_manuals/main/sui/tools/update.sh && chmod +x update.sh && ./update.sh
```

# Logları kontrol ve işlem bu kadar
```
journalctl -u suid -f -o cat
```


# Şimdi Sui Wallet'ı kullanacağız.

* Telegram kanalı: https://t.me/SuiTurkish

* Sui Wallet'ı buradan indiriyoruz: [Wallet Linki](https://chrome.google.com/webstore/detail/sui-wallet/opcgpfmipidbgpenhmajoajpbobppdil/related)

* Daha sonra discorda girip: [Discord](https://discord.gg/8G2SQvwA) #devnet-faucet kanalından oluşturduğumuz cüzdan adresıne token alalım.

* DİKKAT ÇOK HIZLIDIR :)

* Daha sonra Twiter'da paylaşacağım yorumların altında birbirinize Yorumlarda SUİ adresi paylaşarak token gönderin.

* Benim adresim: 0x5c774c3e401f2c3a22dadb8014f843849d053fa1

* Ek olarak NFT 'de gönderelim: Ayarlar kısmından mint NFT demo diyerek mintliyoruz.

* Daha sonra buradan: http://sui-wallet-demo.s3-website-us-east-1.amazonaws.com/ bir NFT oluşturalım ve bunu birbirimize gönderelim.

* Explorer https://explorer.devnet.sui.io/

# Daha sonra discorda giriyoruz ve şu şekilde mesaj atıyoruz #node-ip-application kanalına: https://discord.gg/GUeN8TY7xD

* DAHA ÖNCE ATTIYSANIZ BİR DAHA GEREKLİ DEĞİL ATMANIZ İÇİN

![image](https://user-images.githubusercontent.com/101149671/178118265-a2463048-f656-4382-87cf-faaef1d032d0.png)

Not: #pick-a-role role kanalından da rol alabilirsiniz isterseniz emojilere tıklayarak.

# Nodeunuzu kontrol etmek için: https://node.sui.zvalid.com/

![image](https://user-images.githubusercontent.com/101149671/178118300-29d6bf7e-c78a-40b0-97fd-26bd89d22b05.png)

<h1 align="center"> Yararlı komutlar </h1> 

# Loglar: 
```
journalctl -u suid -f -o cat
```


# Node silmek için:
```
sudo systemctl stop suid
sudo systemctl disable suid
sudo rm -rf ~/sui /var/sui/
sudo rm /etc/systemd/system/suid.service
```

# Node durumunu kontrol:
```
journalctl -u suid -f
```
![image](https://user-images.githubusercontent.com/101149671/178118339-82da6b52-bdb9-425a-af8d-832a671141aa.png)

# Node reset atma:
```
sudo systemctl restart suid
```

# Node durdurma: 
```
sudo systemctl stop suid
```

# Sorun yaşarsanız beni Telegram kanalı: https://t.me/SuiTurkish üzerinden etiketleyin . @Ruesandora kullanıcı adım.
