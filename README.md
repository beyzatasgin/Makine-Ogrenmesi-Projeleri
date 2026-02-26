# Sağlık Alanında Makine Öğrenmesi Projeleri

Bu repository, sağlık alanında 5 farklı makine öğrenmesi projesini içermektedir. Her proje **CRISP-DM metodolojisi** kullanılarak geliştirilmiş ve hem **KNIME** hem de **Python** ile çözülmüştür.

##  Proje İçeriği

Bu repository aşağıdaki 5 makine öğrenmesi projesini içermektedir:

1. **Classification**: Meme Kanseri Hayatta Kalma Tahmini
2. **Regression**: COVID-19 Ölümleri Tahmini
3. **Classification**: Makine Öğrenmesi ile Stres Tespiti
4. **Classification**: Su Kalitesi Analizi
5. **Association Rule / Anomaly Detection**: COVID-19 Aşıları Analizi

##  Proje Gereksinimleri

- Her proje **CRISP-DM metodolojisine** göre başlıklara bölünmüştür
- Problemler hem **KNIME** hem de **Python** ile çözülmüştür
- Her iki çözüm için de dokümantasyon mevcuttur
- Birden fazla model kullanılmıştır
- **Auto ML** kullanılmıştır (Metasezgisel algoritmalarla parametre en iyileme ve en uygun algoritmanın seçilmesi)

##  Proje Yapısı

```
5ML/
│
├── 1.Makine Öğrenmesi ile Meme Kanseri Hayatta Kalma Tahmini/
│   ├── BRCA.csv                          # Veri seti
│   ├── project_1python.ipynb            # Python notebook
│   ├── project-1.knwf                   # KNIME workflow
│   └── project-1.docx                   # Proje dokümantasyonu
│
├── 2. COVID-19 Ölümleri Tahmini/
│   ├── COVID19 data for overall INDIA.csv
│   ├── python.ipynb
│   ├── project-2.knwf
│   └── project-2 .docx
│
├── 3. Makine Öğrenmesi ile Stres Tespiti/
│   ├── stress.csv
│   ├── project_3python.ipynb
│   ├── project-3.knwf
│   └── project-3.docx
│
├── 4-Su Kalitesi Analizi/
│   ├── water_potability.csv
│   ├── project_4.ipynb
│   ├── project_4.knwf
│   └── project-4.docx
│
└── 5-Covid-19 Aşıları Analizi/
    ├── country_vaccinations.csv
    ├── project_5python.ipynb
    ├── project-5.knwf
    └── project-5.docx
```

##  Proje Detayları

### 1. Meme Kanseri Hayatta Kalma Tahmini (Classification)

**Amaç**: Meme kanseri hastalarının hayatta kalma durumunu tahmin etmek

**Veri Seti**: BRCA (Breast Cancer) veri seti
- Hasta bilgileri (Yaş, Cinsiyet)
- Protein seviyeleri (Protein1-4)
- Tümör özellikleri (Tümör evresi, Histoloji)
- Hormon reseptör durumları (ER, PR, HER2)
- Cerrahi tipi

**Kullanılan Teknolojiler**:
- Python: scikit-learn (SVM, diğer sınıflandırma modelleri)
- KNIME: Classification algoritmaları

**CRISP-DM Aşamaları**:
- Business Understanding
- Data Understanding
- Data Preparation
- Modeling
- Evaluation
- Deployment

---

### 2. COVID-19 Ölümleri Tahmini (Regression)

**Amaç**: COVID-19 vakalarına bağlı olarak ölüm sayılarını tahmin etmek

**Veri Seti**: COVID-19 Hindistan veri seti
- Günlük vaka sayıları
- Günlük ölüm sayıları
- Tarih bilgileri

**Kullanılan Teknolojiler**:
- Python: Regression modelleri
- KNIME: Regression algoritmaları

**CRISP-DM Aşamaları**:
- Business Understanding
- Data Understanding
- Data Preparation
- Modeling
- Evaluation
- Deployment

---

### 3. Makine Öğrenmesi ile Stres Tespiti (Classification)

**Amaç**: Metin verilerinden stres durumunu tespit etmek

**Veri Seti**: Stress detection veri seti
- Metin verileri
- Sentiment analizi özellikleri
- Sosyal medya metrikleri

**Kullanılan Teknolojiler**:
- Python: Naive Bayes (BernoulliNB), NLP teknikleri
- KNIME: Text mining ve classification

**CRISP-DM Aşamaları**:
- Business Understanding
- Data Understanding
- Data Preparation
- Modeling
- Evaluation
- Deployment

---

### 4. Su Kalitesi Analizi (Classification)

**Amaç**: Su kalitesini analiz ederek içilebilirlik durumunu belirlemek

**Veri Seti**: Water Potability veri seti
- pH değeri
- Sertlik (Hardness)
- Katı madde miktarı
- Klorür seviyesi
- Sülfat seviyesi
- İletkenlik
- Organik karbon
- Trihalometan seviyesi
- Türbidite

**Kullanılan Teknolojiler**:
- Python: PyCaret (AutoML), Classification modelleri
- KNIME: Classification algoritmaları

**CRISP-DM Aşamaları**:
- Business Understanding
- Data Understanding
- Data Preparation
- Modeling
- Evaluation
- Deployment

---

### 5. COVID-19 Aşıları Analizi (Association Rule / Anomaly Detection)

**Amaç**: COVID-19 aşı verilerini analiz ederek ilişkileri ve anormallikleri tespit etmek

**Veri Seti**: Country Vaccinations veri seti
- Ülke bilgileri
- Aşı tipleri
- Aşı sayıları
- Tarih bilgileri

**Kullanılan Teknolojiler**:
- Python: Association Rule Mining, Anomaly Detection algoritmaları
- KNIME: Association Rule ve Anomaly Detection node'ları

**CRISP-DM Aşamaları**:
- Business Understanding
- Data Understanding
- Data Preparation
- Modeling
- Evaluation
- Deployment

##  Kullanılan Teknolojiler

### Python Kütüphaneleri
- `pandas` - Veri manipülasyonu
- `numpy` - Sayısal hesaplamalar
- `scikit-learn` - Makine öğrenmesi modelleri
- `pycaret` - AutoML
- `plotly` / `matplotlib` / `seaborn` - Görselleştirme
- `nltk` - Doğal dil işleme (Proje 3)

### KNIME
- Classification node'ları
- Regression node'ları
- Clustering node'ları
- Association Rule Mining node'ları
- Anomaly Detection node'ları
- AutoML extension'ları

##  CRISP-DM Metodolojisi

Tüm projeler **CRISP-DM (Cross-Industry Standard Process for Data Mining)** metodolojisine göre yapılandırılmıştır:

1. **Business Understanding**: İş probleminin anlaşılması
2. **Data Understanding**: Veri setinin keşfi ve anlaşılması
3. **Data Preparation**: Veri temizleme ve hazırlama
4. **Modeling**: Model seçimi ve eğitimi
5. **Evaluation**: Model performansının değerlendirilmesi
6. **Deployment**: Modelin dağıtımı ve kullanımı

##  Kurulum ve Kullanım

### Gereksinimler

```bash
pip install pandas numpy scikit-learn pycaret plotly matplotlib seaborn nltk
```

### Projeleri Çalıştırma

1. Her proje klasörüne gidin
2. Python notebook'ları Jupyter veya Google Colab'da açın
3. KNIME workflow dosyalarını KNIME Analytics Platform'da açın
4. Veri setlerini ilgili klasörlere yerleştirin



##  Dokümantasyon

Her proje için ayrıntılı dokümantasyon mevcuttur:
- **Python Notebook**: Kod açıklamaları ve analiz adımları
- **KNIME Workflow**: Workflow açıklamaları ve node yapılandırmaları
- **Word Dokümantasyonu**: Detaylı proje raporu (CRISP-DM metodolojisine göre)



