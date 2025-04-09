-Docker Hub'dan bir imajı nasıl çekersiniz?
docker pull centos 
-Çektiğiniz Docker imajını nasıl çalıştırırsınız?
docker run centos
-Çalışan konteynerları nasıl listeleyebilirsiniz?
docker ps 

-Çalışanlar dahil tüm konteynerları nasıl listeleyebilirsiniz?
docker ps -a 

-Bir çalışan konteynerı nasıl durdurursunuz?
docker stop containerID
-Durdurulmuş bir konteynerı nasıl silersiniz?
docker rm containerID
-Basit bir Dockerfile ile imajı nasıl build edersiniz?
 a- Bir Docker file olusturuyoruz  sonra ilk satir olarak 
 #FROM yazilir burda hangi OS container build edecegimizi bilirliyoruz
 b- RUN command ile OS'in icinde update veya install etmek istedigimiz toolari yaziyoruz. 
 c- WORKDIR ile calisma dizisini olusturuyoruz. 
 d- herhangi bir script veya documanlarimiz varsa COPY command ile calisma dizisine kopyaliyoruz. 
 e- CMD ilede bash veya herhangi bir interactive env olusturuyoruz. 

Docker Build Commands
docker build -t <Name>:<version> .
docker run <name:versin>

-Kendi bilgisayarınızda bir klasör oluşturun. Bu klasör, Python dosyanızı ve Dockerfile'ınızı barındıracak.
Hello.sh adında bir dosya oluşturun.
echo "Hello from Docker!" kodunu ekleyin.
Aynı dizinde Dockerfile adında bir dosya oluşturun.
Dockerfile içinde Ubuntu:22.04 imajı çalışsın.
Docker imajını build edin
Docker imajını çalıştırınls
-Oluşturduğunuz imajı Docker Hub’a nasıl yüklersiniz?
-> docker login / Makineden login yaptiktan sonra dockerfile taglamamiz lazim
-> docker tag dockerfile faruhbek/dockerfile.latest / tagladiktan sonra push etmemiz lazim 
-> docker tag fsubuntu:0.0.8 faruhbek/fsubuntu:0.0.8
docker push  faruhbek/fsubuntu:0.0.8  

-Docker Hub’dan yüklediğiniz imajı başka bir makinede nasıl indirirsiniz?
docker pull faruhbek/dockerfile.latest  
           

-İndirilen Docker imajını nasıl çalıştırırsınız ve konteynerları nasıl listelersiniz?
docker images 
docker run -it faruhbek/dockerfile.latest  

-Bir konteynerın loglarını nasıl görüntülersiniz?
docker logs containerID

Ornek yapabilirmiyiz 
Çalışan bir konteynerın içine nasıl girersiniz?

Docker run -it container ismi 

-Konteynere nasıl dosya taşırsınız

docker cp <path to file> faruhbek/dockerfile.latest/app

-Docker imajını nasıl silersiniz
docker stop contianer id
docker rm container id



GIT HUB

git status - genel bir status gorme
git add <folder> - yeni create edilmis veya modified edilmis klasorler ekle

