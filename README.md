# Centos-7-Docker-Git-Curl-Kurulumu-
**Centos 7'ye Docker, Git ve Curl kurulumu nasıl yapılır**

**Öncelikle İşletim Sistemini Güncelleyelim**
````
yum update -y
````
᲼
᲼
**Docker'ı Kuralım**᲼
````
yum install docker
````

᲼
᲼
**Kurulum Tamamlandıktan Sonra Docker Servisini Çalıştıralım ve Sürekli Hale Getirelim**
````
systemctl start docker
systemctl enable docker
````
᲼
᲼
**Git kurulumu yapalım**
````
yum install git
````
᲼
᲼
**Eğer komut Hatasız bir şekilde biterse git'i kurmuş olursunuz. Ama yinede düzgün çalıştığından emin olmak için bu komutu kullanabilirsiniz**
````
git --version
````
᲼
᲼
**Artık git'i yüklediğinize göre, doğru bilgilerin eklendiği taahhüt mesajlarının oluşturulması için kendinizle ilgili bazı bilgileri yapılandırmanız gerekecek. Bunu yapmak için, taahhütlerinize eklemek istediğiniz adı ve e-posta adresini sağlamak üzere git config komutunu kullanın**
````
git config --global user.name "Kullanıcı ismi"
git config --global user.email "Email adresi"
````
᲼
᲼
**Bu konfigürasyonların başarıyla eklendiğini onaylamak için, ayarlanmış olan tüm konfigürasyon öğelerini yazarak görebiliriz**
````
git config --list
````

**Bu komutu yazdığınızda şu yanıtı alıcaksınız**
```
user.name="Kullanıcı ismi"
user.email="Email adresi"
```
᲼
᲼**Şimdide Curl kurulumu**
````
yum install curl
````
