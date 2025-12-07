# 📈 Python ile Uçtan Uca Kişisel Finans Analizi

## 🌟 Proje Amacı ve Motivasyon
Bu proje, sentetik olarak üretilmiş düzensiz finansal verileri (harcamalar) alıp, Pandas ve NumPy kullanarak bu verileri anlamlı içgörülere dönüştürmeyi ve portfolyoda **gerçek dünya veri mühendisliği** yeteneğini sergilemeyi amaçlamaktadır. Proje, popüler Titanic/Iris setleri yerine, **pratik ve ölçeklenebilir** bir finansal analiz süreci sunar.

## ⚙️ Kullanılan Teknolojiler
* **Python** (3.x)
* **Pandas:** Veri manipülasyonu, Feature Engineering, `groupby`, `resample`.
* **NumPy:** Yüksek performanslı vektörel işlemler ve gerçekçi harcama simülasyonu (`np.random.normal`).
* **Matplotlib:** Analitik sonuçların görselleştirilmesi.
* **Jupyter Notebook:** Uçtan uca analitik akış.

## 🔬 Metodoloji ve Analitik Adımlar

Proje, aşağıdaki 5 ana aşamada ilerlemiştir:

1.  **Veri Simülasyonu:** Normal dağılım ve ağırlıklı rastgele seçim ile gerçekçi harcama verisi üretimi.
2.  **Veri Temizliği:** Kasıtlı NaN oluşturma ve Koşullu Veri Doldurma (`np.select()`) ile eksik veri yönetimi.
3.  **Özellik Mühendisliği (Feature Engineering):** Tarih indeksinden `'Gun Adi'`, `'Ay_Donemi'` ve `'Hafta_Turu'` gibi analitik sütunların türetilmesi.
4.  **İleri Finansal Metrikler:**
    * Kategori bazlı özetler (`groupby.agg`).
    * Aylık harcama trendi (`resample`).
    * **Aydan Aya Büyüme (MoM)** analizi.
    * Kategori bazlı mevsimselliği gösteren **Pivot Tablolar**.
5.  **Görselleştirme:** Harcama trendi ve kategori dağılımı grafikleri.

## 📊 Çıkan Kritik İçgörüler
* [assets/kategori_dagilimi_grafigi.png] (Grafik görseli buraya gelecek)
    * *Örn: "Toplam harcamaların %45'i Market ve Fatura kategorilerinde yoğunlaşmaktadır."*
* [assets/aylik_harcama_trend_grafigi.png] (Grafik görseli buraya gelecek)
    * *Örn: "MoM analizi, yılın son çeyreğinde (Ekim-Aralık) harcamalarda ortalama %12'lik bir artış trendi olduğunu göstermiştir."*

## 🛠️ Kurulum ve Çalıştırma
Projeyi yerel olarak çalıştırmak için aşağıdaki adımları takip edin:

```bash
# 1. Depoyu Klonlayın
git clone https://github.com/selejder/Finansal-Veri-Projesi
cd Finansal-Analiz-Projesi

# 2. Bağımlılıkları Kurun
pip install -r requirements.txt

# 3. Notebook'u Başlatın
jupyter notebook FinansalVeriProjesi.ipynb
```
## Not
Projenin hazırlanmasında Google'ın Gemini 3 modeli kullanılmıştır.
