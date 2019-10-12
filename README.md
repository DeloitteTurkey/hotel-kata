# Günün Programı
09:00 - 09:30  Tanışma, Çay - Kahve <br/>
09:30 - 11:00  Domain Story Telling (DST) yönetimi ve DDD ile ilişkisi <br/>
11:00 - 12:00  Örnek bir senaryo üzerinden DST çalışması <br/>
12:00 - 12:45  Yemek arası <br/>
13:00 - 17:00  DDD odaklı kodlama ve DST ek senaryolar ile kod değişiklikleri çalışması<br/>
17:00 - 17:30  Retrospective <br/>
<br/>

DST TOOL: https://www.wps.de/modeler/

# Domain Story Telling Nedir? <br/>
https://domainstorytelling.org/ <br/>
<br/>


# Domain Driven Design Nedir? <br/>
* https://www.infoq.com/minibooks/domain-driven-design-quickly/#minibookDownload/
* https://developer.ibm.com/tutorials/reactive-in-practice-1/ (alternatif bir teknik olan event storming ile anlatım)
* https://docs.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/ddd-oriented-microservice
* https://docs.microsoft.com/bs-latn-ba/azure/architecture/microservices/model/tactical-ddd
* https://learning.oreilly.com/library/view/patterns-principles-and/9781118714706/
<br/>




# Otel Rezervasyonu DST Katathon <br/>

Başlangıç Senaryosu: <br/>
1. Otele müşteri geldi, 17-20 Temmuz arası 2 kişilik oda ayırmak istedi.
1. Çalışan önündeki programdan bu zaman aralığındaki müsait odaları aradı.
1. Sistem müsait oda listesini döndü.
1. Çalışan bu listeyi müşteriye önermeye başladı. (Bu noktada müşteri listeden rastgele bir oda seçtiği kabul edilebilir)
1. Müşteri odayı seçti ve ayırmak istedi.
1. Çalışan sistem üzerinden odayı ayırma işlemini başlattı.
1. Oda başarıyla ayrılınca çalışan müşteriye odanın onaylandığında dair bilgi verdi.
<br/>

Başlangıç Domain Kuralları: <br/>
* Otelde toplam 100 oda bulunuyor
* Şu anda sadece "standart" oda tipi mevcut.
* Odaların %20'si 3 kişilik, %60'ı 2 kişilik, %20'si 4 kişiliktir.
* Odaların hepsi her sezon müsait.
* Standart oda kişi başı fiyat 50 tl.
* Her yaş için ücret alınıyor.
* Eğer verilen tarihte müsait oda olmazsa, önce tarihi 1 gün ileri/geri oynatıyorum ve oda müsaitlik durumuna bakıyorum. Eğer bu tarihler misafir için uygun olmazsa orjinal süreyi bölüp alternatif odalar öneriyorum.
<br/>


# TDD Kaynakları <br/>
* https://hackernoon.com/introduction-to-test-driven-development-tdd-61a13bc92d92
* https://www.ibm.com/developerworks/java/library/j-eaed2/index.html
<br/>

