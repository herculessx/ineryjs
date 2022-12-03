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

4. Yeni env dosyası oluşturun ve düzenleyin

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


## 🟢 Çalıştırma

RPC Örneği Çalıştır

```
npm run rpc-example
```

işlem çıktısı aşağıdaki gibi olmalı<br>
<img src="https://raw.githubusercontent.com/herculessx/Q-Network-Testnet/main/inery-okey.PNG" width="750">
