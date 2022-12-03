## 🟢 Inery Json RPC 4.Görev
Inery Blockchain'de JSON RPC'yi çağırmak için örnek bir kod

## 🟢Bilgiler

JSON RPC Örnek kodu örnek dizinde mevcuttur, [example](https://github.com/herculessx/ineryjs/blob/master/example/) değiştirmeyi deneyebilir ve nasıl çalıştığını anlayabilirsiniz, ayrıca kodunuzu çalıştırabilmek ve değerli sözleşme işlevini çağırabilmek için Hesabınızda Değerli Akıllı Sözleşmeye (Görev 3) sahip olmanız gerekir.


## 🟢 Başlayın
Eski Nodejs kaldırın
<br>

```shell
sudo apt-get remove nodejs
```

Curl'ü yükleyin

```shell
sudo apt-get install curl
```

Curl'ü yükleyin

```shell
    curl -fsSL https://deb.nodesource.com/setup_19.x | sudo -E bash - &&\
    sudo apt-get install -y nodejs
```

     
## 🟢 NPM kurulumu

```shell
sudo apt install npm
```



## 🟢 Kurulum

1. Repoyu klonlayın

   ```
   git clone https://github.com/herculessx/ineryjs.git
   ```

2. Dizine Girin

   ```
   cd ineryjs
   ```

3. NPM Paket kurun

   ```
   npm install
   ```

4. Aşağıdaki Kod ile env-sample dosyasının ismini .env yapın 

   ```
   cp .env-sample .env
   ```

5.  ```.env``` bilgileriniz düzenleyin

  ```
   nano .env
   ```

Burada açılan pencerede <br>

INERY_ACCOUNT=  İnery hesap isminiz <br>
PRIVATE_KEY="keyiniz"<br>
NODE_URL="http://NODEİPADRESİ:8888" 
<br><br>

ctrl +X  Yes diyip çıkıyoruz.


<br>
<img src="https://raw.githubusercontent.com/herculessx/Q-Network-Testnet/main/env-duzenle.png" >

## 🟢 8888 port açma 

RPC Örneği Çalıştır

```
sudo ufw allow 8888
```

<br>
## 🟢 Çalıştırma

RPC Örneği Çalıştır

```
npm run rpc-example
```

işlem çıktısı aşağıdaki gibi olmalı<br>
<img src="https://raw.githubusercontent.com/herculessx/Q-Network-Testnet/main/inery-okey.PNG" width="750">


<br><br>
## 🟢 Hata Çözümleri

Serialization time limit 15000us exceeded

<br>
config.ini dosyanda max-transaction-time değerini 15000 olarak değiştir 

```
nano ./inery-node/inery.setup/master.node/blockchain/config/config.ini
```

<img src="https://camo.githubusercontent.com/6036fa176fe713bfa7e8151aef13b77710b589c33dff2f7ae459d2b8785e0efc/68747470733a2f2f736e6970626f6172642e696f2f61306472474e2e6a7067" width="550">
