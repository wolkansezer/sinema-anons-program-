# sinema-anons-program-
SİNEMALARDA KULLANILMASI İÇİN TASARLADIĞIM ANONS PROGRAM 

SINETECHNİC VOLKAN SEZER  YAŞIM 35 17 YILDIR SİNEMA SEKTÖRÜNDEYİM  

PROGRAM AÇIKLAMASI 

Sinema anons programının çalışma mantığı ve açıklaması aşağıdaki gibidir:

1. **IP Tetikleme Dinleyicisi (IPTriggerListener)**: Bu bileşen, belirli bir IP adresi ve port üzerinden gelen tetikleme sinyallerini dinler. Tetikleme sinyali geldiğinde, bir geri çağırma fonksiyonu (trigger_callback) çağrılır.

2. **Anons Yöneticisi (AnnouncementManager)**: Bu bileşen, sinema salonlarına yönelik başlangıç ve ara anonslarını yönetir. Başlangıç ve ara anonsları için ses dosyalarını yükler ve bunları çalıştırma işlevlerini sağlar. Ayrıca ses seviyesini ayarlama özelliği de bulunmaktadır.

3. **Otomasyon Entegrasyonu (AutomationIntegration)**: Bu bileşen, IPTriggerListener ve AnnouncementManager bileşenlerini birbirine bağlar. Tetikleme sinyali geldiğinde, ilgili salon için başlangıç ve ara anonslarının çalınmasını sağlar.

4. **Kullanıcı Arayüzü (AnnouncementGUI)**: Bu bileşen, Tkinter kullanarak bir kullanıcı arayüzü oluşturur. Arayüzde şu özellikler bulunmaktadır:
   - Salon ve ARA butonları: Kullanıcının manuel olarak anonsları başlatmasını sağlar.
   - Sunucu IP ve Port girişi: Kullanıcının IP tetikleme dinleyicisinin IP adresi ve portunu ayarlamasını sağlar.
   - Ses seviyesi ayarı: Kullanıcının anons sesini ayarlamasını sağlar.
   - Müzik çalar bağlantıları: Kullanıcının YouTube ve Spotify gibi müzik platformlarına erişmesini sağlar.
   - IP değişikliği takip kutusu: IP adresi değişikliklerini gösterir.
   - Program sahibi ve e-posta bilgileri.

Uygulama, IPTriggerListener bileşeni aracılığıyla belirli bir IP adresi ve port üzerinden gelen tetikleme sinyallerini dinler. Tetikleme sinyali geldiğinde, AnnouncementManager bileşeni kullanılarak ilgili salon için başlangıç ve ara anonsları çalınır. Kullanıcı arayüzü, kullanıcının manuel olarak anonsları başlatmasına, ses seviyesini ayarlamasına ve diğer özellikleri kullanmasına olanak sağlar.

Bu yapı, sinema anons programının farklı bileşenlerini modüler ve yeniden kullanılabilir hale getirerek, uygulamanın esnekliğini ve bakımını kolaylaştırır.
