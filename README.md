# MEME KANSERİNİN TAHMİNİ
Meme kanseri (BC), dünya çapında kadınlar arasında en yaygın kanserlerden biridir ve küresel istatistiklere göre yeni kanser vakalarının ve kansere bağlı ölümlerin çoğunu temsil etmektedir.

Bu depoda kullandığım veri seti kamuya açıktır ve Madison, Wisconsin, ABD'deki Wisconsin Üniversitesi Hastanesi doktoru Dr. William H. Wolberg tarafından oluşturulmuştur. 
bağlantı:https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data

Bu modelde bir meme tümörü örneğinin iyi huylu mu yoksa kötü huylu mu olduğunu tahmin etmek için SVM ve KNN algoritmalarını kullandık. Bu süreçte varsayılan parametrelere sahip modeller oluşturduk ve ardından bunları optimize etmek için teknikler kullandı.Bu veri kümesi 596 örneğe ve ortalama yarıçap, ortalama doku, ortalama parametre, ortalama düzgünlük vb. gibi 30 özelliğe sahiptir. 

## Veri İçeriği
Hasta durumu tahmin etme? -iyi huy kötü huy tahmin etme?
#### Attribute Information(Öznitelik Bilgileri)
- ID number
- Diagnosis (M = malignant(kötü huylu), B = benign)
#### Ten real-valued features are computed for each cell nucleus
Her hücre için 10 gerçek değerli özellik hesaplanır.

- radius (mean of distances from center to points on the perimeter)
Yarıçap (hücre çeperinden çekirdeğe ortalama uzaklık)

- texture (standard deviation of gray-scale values)
Doku (gri-ölçek değerlerin standart sapması)

- perimeter(çevre)
Hücrelerin çevre uzunlukları ortalaması, standart sapması ve
en kötü değeri

- area(alan)
Hücrelerin yüzey alanları ortalaması, standart sapması ve en kötü
değeri

- smoothness (local variation in radius lengths)
Düzgünlük (hücre çekirdeğine olan uzunluktaki farklılık)

- compactness (perimeter^2 / area - 1.0)
Sıklık Çevre²/(Alan-1)

- concavity (severity of concave portions of the contour)
Dışbükeylik


- concave points (number of concave portions of the contour)
Dışbükey noktalar (dışbükey alanların hücre çeperine oranı)

- symmetry
Simetri

- fractal dimension ("coastline approximation" - 1)
Fraktal boyutu
İç içe geçmiş düzensiz hücrelerin tüm normal
hücrelere oranının ortalaması, standart sapması ve en kötü değeridir.

Meme kanseri olanlarda ölüm nedenine yapılan atıflar, hastanın özelliklerine bağlı birçok nedene bağlı olabilir. Herhangi bir spesifik neden meme kanseri sonucu ölüm riskini azaltabilir. Bununla birlikte, bu sonuçlar hem aktif hem de eski meme kanseri öyküsü olan hastaların karşılaştıkları erken teşhisin öneminin altını çizmektedir. Çalışmamız meme kanserli kadınlarda erken tanının yüksek doğrulukla yapılmasının önemini pekiştirmektedir.