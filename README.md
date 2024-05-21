# TableView-Kent-Simgeleri

Bu Swift kodu, bir UITableView kullanarak belirli yer işaretlerini (landmark) listeleyen ve kullanıcıların bu yer işaretlerini seçerek detaylarını görüntüleyebileceği bir iOS uygulaması oluşturuyor. Kod, temel olarak bir UIViewController sınıfını genişletir ve UITableViewDelegate ve UITableViewDataSource protokollerini uygular.

# Özellikler:

# Veri Kaynakları:

# landmarkNames: Yer işaretlerinin isimlerini tutar.
# landmarkImages: Yer işaretlerinin görüntülerini tutar.
# chosenLandmarkName: Seçilen yer işaretinin adı.
# chosenLandmarkImage: Seçilen yer işaretinin görüntüsü.


# View Did Load:

tableView için delegate ve dataSource atanır.
landmarkNames ve landmarkImages dizileri doldurulur.

# UITableViewDataSource:

tableView(_:numberOfRowsInSection:): Satır sayısını landmarkNames dizisinin eleman sayısı olarak döner.
tableView(_:cellForRowAt:): Her bir hücreyi yer işareti adıyla doldurur.

# UITableViewDelegate:

tableView(_:didSelectRowAt:): Bir satır seçildiğinde, seçilen yer işaretinin adı ve görüntüsü atanır ve detaylar sayfasına geçiş yapılır (performSegue).
prepare(for:sender:)

Geçiş işlemi sırasında seçilen yer işaretinin adı ve görüntüsü, hedef ViewController'a (detailsVC) aktarılır.
Silme İşlevi:

tableView(_:commit:forRowAt:): Kullanıcı bir satırı sildiğinde, ilgili yer işareti adı ve görüntüsü dizilerden kaldırılır ve tablo güncellenir.

<h2>Ekran Görüntüsü</h2>

![yeni (1)](https://github.com/Sabricetin/TableView-Kent-Simgeleri/assets/114506296/0d49b657-cfce-4f59-a0d6-55ee9988127a)

