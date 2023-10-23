<h1 align="center">Pactus</h1>

> `500 kişi` ile sınırlıdır - Ödül `100 PAC` tokenidir - Çok düşük donanıma sahiptir

>  Ne zaman bitecek bilinmiyor - Taşıması çok kolay

> Önemli linkler: [Duyuru](https://t.me/RuesAnnouncement) - [Sohbet](https://t.me/RuesChat) -  [WP Kanalı](https://whatsapp.com/channel/0029VaBcj7V1dAw1H2KhMk34) - [Discord](https://discord.gg/TSMpzxZnre)

> Sağ üstten `fork` & `yıldız` yapmayı unutmayın!


<h1 align="center">Donanım</h1>

> Yeni sunucu almadım, hali hazırda `8080` portu kullanmayan bir sunucu kullandım.

> [Hetzner](https://github.com/ruesandora/Hetzner) kullanıyorum.

```console
# Minimum
1 CPU 1 RAM - Ubuntu 22

# Port kontrol
lsof -i -P -n | grep LISTEN
```

<h1 align="center">Kurulum</h1>

```console
sudo apt update -y && sudo apt upgrade -y
sudo apt install screen

curl --proto '=https' --tlsv1.2 -sSL  https://github.com/pactus-project/pactus/releases/download/v0.15.1/pactus_downloader.sh | sh

cd pactus-cli_0.15.1

# 12 kelimenizi alın ve şifrenizi yedekleyin.
./pactus-daemon init -w ~/pactus --testnet
# 7 sayısına enter diyin - çıktıyı yedekleyin

screen -S pactus
./pactus-daemon start -w ~/pactus
# sync olmasını bekleyin, explorer: https://explorer.codeblocklabs.com/pactus/validator.php
```

> Sync olduktan sonra `1. validatör` adresine `token` isteyin.

> Bu aşamada bu adresinize otomatik `delege` edilecek ve `discord=validatör` bağlantısı yapılacak

> Diğer adresler içinde validatör kurmak istiyorsanız 1. adresinize gelen token rewards ile diğer validatörlere stake edersiniz

> Ödül birikmedi bende de birikince buraya eklerim o kısmıda.




