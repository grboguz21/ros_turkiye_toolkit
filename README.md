# ROS Türkiye Toolkit
ursa devam etmeden önce, proje geliştirme süreci için bir ortam oluşturmamız gerekiyor. Programlamada biz bu ortamlara sanal ortam (virtual environment) diyoruz.

Bunun için aşağıdaki adımları videoyu da izleyerek takip ediniz:

1. Anaconda Kurulumu 

Terminali açın (Ctrl+Alt+T) ve şu komutları sırasıyla uygulayın:





Yükleyiciyi İndirin:

wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh





Kurulumu Başlatın:

bash Miniconda3-latest-Linux-x86_64.sh 

(Kurulum sırasında Enter tuşuna basın, lisans metnini q ile geçin ve onay istendiğinde yes yazın.)





Terminali Yenileyin: Değişikliklerin aktif olması için terminali kapatıp açın veya şu komutu çalıştırın:

~/miniconda3/bin/conda init bash
source ~/.bashrc



Kurulumu Doğrulayın: Mevcut terminaliniz kapatıp, yeni bir terminal açın. Ardından ekranda (base) ibaresini görüyorsanız kurulum başarıyla tamamlanmıştır.



2. Anaconda Ortamı Oluşturma ve Gerekli Kütüphanelerin Kurulumu 

Anaconda Prompt’u açın ve sanal ortamınızı oluşturun. Kendi örneğimde bu ortamı ros_turkiye olarak adlandırdım.



Önemli Not: Bu kılavuzda belirtilen kütüphaneleri ve kütüphane versiyonlarını birebir aynı şekilde kurduğunuzdan emin olun. Belirtilenden farklı veya daha yeni Python sürümleri kullanmaktan kaçının; aksi takdirde gerekli bazı kütüphanelerle uyumluluk sorunları yaşayabilirsiniz.

Sırasıyla Uygulamanız Gereken Komutlar:





Sanal Ortamı Oluşturun: Python 3.13 sürümü ile ros_turkiye adında yeni bir ortam yaratın.

conda create -n ros_turkiye python=3.13  



Ortamı Aktif Hale Getirin: Oluşturduğunuz ortama giriş yapın.

conda activate ros_turkiye



Gerekli Kütüphaneleri Yükleyin: Projenin çalışması için ihtiyaç duyulan tüm bağımlılıkları (YOLO, OpenCV vb.) uzak sunucudaki listeden otomatik olarak kurun.

pip install -r https://raw.githubusercontent.com/grboguz21/ros_turkiye_project/refs/heads/main/requirements.txt



3. Visual Studio Code ile Kodlamaya Başlayın 

Artık Bilgisayarlı Görü (Computer Vision) kütüphaneleriniz kuruldu ve kod yazmaya hazırsınız. 

Kendi Python projenizi oluşturmak amacıyla VS Code’u kurmak ve yapılandırmak için bir doğrudan bu derse geçebilirsiniz: 

🧑‍💻 Visual Studio Code - Tıkla Çalıştır ! 



Not: Eğer kurulum aşamasında hata ile karşılaştıysanız: ❓Kurulum Hataları
