<h1 align="center"> Opside | Pre-Alpha Testneti 
  
## Opside Ödüllü testnet formunu doldurmuştuk. Formu dolduranlar için kazanıp kazanmadığını öğrenmek için;
  * [BURADAN](https://discord.gg/opside) Opside discord kanalına gidiyoruz.
  * Faucet kanalında #for-validator kanalına @Opside Faucet ekleyip, formu doldurduğunuz Metamask adresinizi veriyoruz. Seçildiyseniz cüzdanınıza 25001 IDE test tokeni gelecek, seçilmediyseniz. "You are not qualified for Validators, please participate in the new round of validator application activities." şeklinde uyarı alacaksınız.


## Sistem gereksinimleri:
NODE TİPİ | CPU     | RAM      | SSD     |
| ------------- | ------------- | ------------- | -------- |
| Opside  | 4          | 16         | 500  |
  

# Kurulum

```
sudo apt-get update -y && sudo apt-get upgrade -y
```

```
sudo apt install -y build-essential libssl-dev cmake screen git htop
```
### Opside Yüklüyoruz.
```
wget -c https://pre-alpha-download.opside.network/testnet-auto-install-v2.tar.gz 
tar -C ./ -xzf testnet-auto-install-v2.tar.gz
chmod +x -R ./testnet-auto-install-v2
cd ./testnet-auto-install-v2
```
### Genesis Dosyalarını yüklüyoruz.
```
wget -c https://pre-alpha-download.opside.network/testnet-auto-install.tar.gz 
tar -C ./ -xzf testnet-auto-install.tar.gz
chmod +x -R ./testnet-auto-install
cd ./testnet-auto-install
```

### Node Başlatalıyoruz.
* Bu işlemi yaptıktan sonra;
```
./install-ubuntu-en-1.0.sh
```
* Sırasıyla;
  * Formu doldururken verdiğimiz Metamask cüzdan adresini giriyoruz
  * Bizden şifre isteyecek istediğiniz en az 8 karakterli şifreyi giriyoruz.
  * Tekrar cüzdan adresimizi giriyoruz.
  * Aynı şifreyi tekrar giriyoruz.
  * Bize 12 Kelime verecek bunları alıp bir yere not edin. 
  * Verdiği kelimeleri tekrar giriyoruz.
  
 ### Validator Oluşturma
* Node Sync olup olmadığını aşağıdaki komutlar ile bakabilirsiniz. Aşağıdaki görselde olduğu gibi bloklar akıyorsa sorun yoktur.
 ```
cd ./testnet-auto-install-v2
```
 ```
cd ./testnet-auto-install
```
 ```
opside-chain/show-geth-log.sh
```
![loglar](https://github.com/CoinHuntersTR/opside-testnet-rehberi/assets/111747226/6d1344ea-598d-4e4f-a808-51d068136ca8)

* Blok zincirin en son hangi blokta olduğunu görmek için [BURADAN](https://pre-alpha.opside.info/) kontrol edebilirsiniz.

### Node Sync Olduktan Sonra
 
* [BURADAN](https://opside.network/validator/deposit) validator sitesine ulaşıyoruz. Cüzdanımızı siteye bağlıyoruz.
  
![68747470733a2f2f692e6962622e636f2f53506d567a38502f696d6167652e706e67](https://github.com/CoinHuntersTR/opside-testnet-rehberi/assets/111747226/f14aa7ea-aa6f-48ef-9b18-14d5a2b817f5)
 
 * Buradaki size bazı sorular ve bilgiler veriyor bunları tek tek "Contuine" diyerek kabul ediyoruz. 
  
 * En soon yukarıdaki görseldeki gibi Upload sayfasına geliyoruz. Buraya yükleyeceğimiz dosyayı almak için;
  
 * Mobax üzerinde solda bulanan dosyalar içinden testnet-auto-install-v2 adlı dosyaya giriyoruz.
  
 ![mobax1](https://github.com/CoinHuntersTR/opside-testnet-rehberi/assets/111747226/3b09362e-8ba9-4ee7-a3b1-c8c91fab6d4a)
  
 * testnet-auto-install-v2 dosyası için validator_keys klasörünü açıyoruz.
 
 ![mobax2](https://github.com/CoinHuntersTR/opside-testnet-rehberi/assets/111747226/1a1e8624-c325-4454-be0d-88585514d59f)
  
 * validator_keys klasörü içindeki Deposit data dosyasını sürürkle bırak ile masaüstüne taşıyoruz.
 
 ![mobax3](https://github.com/CoinHuntersTR/opside-testnet-rehberi/assets/111747226/073e21f2-954e-4ec1-8b5e-1fe0706a9f2c)
  
 * Masaüstüne aldığımız dosyayı aşağıdaki yere Upload ettikten sonra; cüzdanımızdan 25000 IDE tokeni stake ediyoruz.

 ![68747470733a2f2f692e6962622e636f2f53506d567a38502f696d6167652e706e67](https://github.com/CoinHuntersTR/opside-testnet-rehberi/assets/111747226/f14aa7ea-aa6f-48ef-9b18-14d5a2b817f5) 
  
  ### Sonuç
  * Tüm adımları doğru şekilde tammamladıktan sonra; 
  ![sonuc](https://github.com/CoinHuntersTR/opside-testnet-rehberi/assets/111747226/2fb5edb9-1c2c-4e02-a516-06b26b6045a0)
  
  Bu şekilde sonuç alacaksınız.
  
