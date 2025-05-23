# Marketplace-Stack

Bu proje, Spring Boot tabanlı bir mikroservis uygulamasını, 
Apache Kafka, Mysql ve Elasticsearch gibi temel altyapı bileşenleriyle bir araya getiren bir Docker Compose yığınıdır.

---

## Kurulum ve Başlatma

Projeyi yerel geliştirme ortamınızda hızlıca ayağa kaldırmak için aşağıdaki adımları izleyin:

### 1. Projeyi Klonlayın

Öncelikle projenin ana deposunu klonlayın:

```bash

git clone git@github.com:erdalceylan/marketplace-stack.git
cd marketplace-stack
```
### 2. Alt Modülleri Başlatın ve Güncelleyin
   Bu proje, bazı bağımlılıkları Git alt modülleri aracılığıyla yönetmektedir.
Bu alt modülleri başlatmak ve en güncel hallerine getirmek için aşağıdaki komutları çalıştırın:
```bash

git submodule update --init --recursive
git submodule update --remote --recursive
```

### 3. Docker Compose ile Başlatın
   Tüm servisleri Docker Compose kullanarak tek bir komutla ayağa kaldırabilirsiniz:
```bash

docker compose up -d
```

### Not
trendyol üzerinden ürünleri çekerek sistemi deneyebilirsiniz.

 ```bash
 
java -jar build/libs/core-0.0.1-SNAPSHOT.jar Fill-Dummy-Data-Trendyol
 ```
