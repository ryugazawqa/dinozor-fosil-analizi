# 🦖 Dinozor Fosil Analizi

Mezozoik dönemine ait dinozor fosil kayıtları üzerinde keşifsel veri analizi (EDA). Fosillerin kıtalara, jeolojik dönemlere ve atmosferdeki oksijen seviyesine göre dağılımını inceler.

## Veri seti

Kaggle'daki **DinoOxyLenght** veri seti (`dinozor_verisi_tam_database.csv`), 809 fosil kaydı içerir.

| Sütun | Açıklama |
|---|---|
| `dinosaur_name` | Takson adı |
| `early_interval`, `late_interval` | Jeolojik zaman aralığı |
| `early_age_mya` | Fosilin yaşı (milyon yıl önce) |
| `country_code`, `continent` | Bulunduğu ülke ve kıta |
| `length` | Vücut uzunluğu (m) |
| `oxygenLevel` | Dönemin atmosferik oksijen seviyesi (%) |

## Yapılan analizler

1. **Kıtalara göre dinozor grubu yoğunluğu:** Takson adlarındaki anahtar kelimelere göre basit bir *Saurischia / Ornithischia* gruplandırması ve ısı haritası.
2. **Dönem ve oksijen seviyesine göre boy:** Kretase, Jura ve Trias dönemlerinde oksijen seviyesine göre fosil sayısı, ortalama ve maksimum boy tablosu.
3. **Fosil yaşlarının dağılımı:** Histogram (MYA).
4. **Kıtalara göre en eski fosil kayıtları:** Yatay çubuk grafik.
5. **Fosil kayıtlarının kıtalara göre payı:** Halka grafik.

## Bazı bulgular

- Kayıtların yarısı Kuzey Amerika'dan (404), ardından Asya (205) ve Güney Amerika (89) geliyor.
- Afrika'dan yalnızca 2 kayıt var. Bu durum dinozorların dağılımından çok veri setindeki örnekleme yanlılığını gösteriyor.

## Çalıştırma

Notebook Kaggle ortamında hazırlandı. Kaggle'da yeni bir notebook açıp **DinoOxyLenght** veri setini girdi olarak ekleyin, ardından `dinozor_fosil_analizi.ipynb` dosyasını içe aktarın.

Kullanılan kütüphaneler: `pandas`, `numpy`, `matplotlib`, `seaborn`
