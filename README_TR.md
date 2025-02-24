# Turkish-NLP-QA-Dataset (SQuAD Format)

Türkçe | [English](README.md)

Bu veri seti, Türkiye'deki tarihi mekanlar ve gezilecek yerler hakkında soru-cevap çiftleri içeren, SQuAD formatında hazırlanmış bir Türkçe doğal dil işleme veri setidir. Veri seti toplamda 15.000 adet QA çifti içermektedir.

## 📝 Veri Seti Hakkında

Bu veri seti, Google Gemini AI kullanılarak oluşturulmuş olup Tamamen Doğrulanmış verilerden oluşturulmuştur Google Gemini modeli ile sadece SQUAD formatına getirilmiştir, Türkiye'nin tarihi ve turistik mekanları hakkında kapsamlı bir soru-cevap koleksiyonu sunmaktadır. Veri seti, makine öğrenimi ve doğal dil işleme çalışmaları için özel olarak SQuAD (Stanford Question Answering Dataset) formatında hazırlanmıştır.

### 🔍 Veri Seti İçeriği

Veri seti aşağıdaki kategorilerdeki yapılar hakkında bilgiler içermektedir:
- Tarihi Hamamlar
- Antik Kentler ve Nekropoller
- Kümbetler ve Anıt Mezarlar
- Sivil Mimari Örnekleri (Konaklar ve Evler)
- Tarihi Kamu Binaları

### 📊 Veri Seti Özellikleri

- **Format**: SQuAD (Stanford Question Answering Dataset)
- **Dil**: Türkçe
- **Konu**: Türkiye'deki tarihi mekanlar ve gezilecek yerler
- **Veri Tipi**: Soru-Cevap çiftleri
- **Kaynak**: Google Gemini AI ile oluşturulmuş içerik

## 🎯 Örnek Veriler

### Örnek 1: Kozlu Ören Yeri (Kırıkkale)
```json
{
  "context": "Kırıkkale İli, Sulakyurt İlçesi'ne tahminen 7 km. uzaklıkta bulunan ve tarla yollarıyla ulaşılan, ayakta hiçbir yapı kalıntısı bulunmayan eski kent kalıntısıdır...",
  "qas": [
    {
      "question": "Kozlu Ören Yeri'nin hangi döneme ait olduğu düşünülmektedir?",
      "answer": "Roma Dönemi"
    },
    {
      "question": "Kozlu Ören Yeri'ne nasıl ulaşılır?",
      "answer": "tarla yollarıyla"
    }
  ]
}
```

### Örnek 2: Emir Ali Kümbeti (Bitlis)
```json
{
  "context": "Bütünüyle dıştan 9.10X 6.05 ebatlarında olan Emir Ali Kümbet'in...",
  "qas": [
    {
      "question": "Kümbetin planı nasıl bir şekildir?",
      "answer": "dikdörtgen"
    },
    {
      "question": "Emir Ali Kümbetinin dış boyutları nelerdir?",
      "answer": "9.10X 6.05"
    }
  ]
}
```

### Örnek 3: Kazım Civciv Evi (Denizli)
```json
{
  "context": "Denizli İli, Serinhisar İlçesi'nde bulunan konut; iki katlı, temelde taş, üst katlarda kerpiç malzeme ile inşa edilmiştir...",
  "qas": [
    {
      "question": "Evin yapımında kullanılan malzemeler nelerdir?",
      "answer": "temelde taş, üst katlarda kerpiç"
    },
    {
      "question": "Evin plan tipi nasıldır?",
      "answer": "açık sofalı"
    }
  ]
}
```

## 🛠️ Veri Seti Oluşturma Süreci

Veri seti, aşağıdaki adımlar izlenerek oluşturulmuştur:

1. Excel formatında ham verilerin toplanması
2. Google Gemini AI kullanılarak içeriklerin işlenmesi
3. Her 500 kayıtta JSON formatında çıktıların oluşturulması
4. Verilerin SQuAD formatına dönüştürülmesi
5. Kalite kontrol ve düzenleme

## 📊 Veri Seti Yapısı

Veri seti JSON formatında olup, her bir kayıt şu bilgileri içermektedir:

```json
{
    "version": "v2.0",
    "data": [
        {
            "title": "context_title",
            "paragraphs": [
                {
                    "context": "Metin içeriği",
                    "qas": [
                        {
                            "question": "Soru metni",
                            "id": "benzersiz_id",
                            "answers": [
                                {
                                    "text": "Cevap metni",
                                    "answer_start": integer
                                }
                            ]
                        }
                    ]
                }
            ]
        }
    ]
}
```

## 🎯 Kullanım Alanları

- Türkçe Doğal Dil İşleme modelleri eğitimi
- Soru-Cevap sistemleri geliştirme
- Tarihi ve kültürel miras bilgi sistemleri
- Turizm uygulamaları
- Eğitim materyalleri geliştirme

## 📦 Gereksinimler

Veri setini oluşturmak için kullanılan kütüphaneler:

- Python 3.x
- pandas
- google.generativeai
- json
- logging

## 🤝 Katkıda Bulunma

Veri setine katkıda bulunmak için:

1. Fork yapın
2. Yeni bir branch oluşturun
3. Değişikliklerinizi commit edin
4. Pull request gönderin

## 📄 Lisans

Bu veri seti GNU General Public License v3.0 (GPL-3.0) altında lisanslanmıştır. Bu lisans size şu hakları verir:
- Veri setini ticari amaçla kullanabilirsiniz
- Veri setini değiştirebilirsiniz
- Veri setini dağıtabilirsiniz
- Veri setini patentleyebilirsiniz
- Veri setini özel kullanım için kullanabilirsiniz

Daha fazla detay için [LICENSE](LICENSE) dosyasını veya [GNU GPL v3.0](https://www.gnu.org/licenses/gpl-3.0.tr.html) sayfasını ziyaret edin.

## 📞 İletişim
# Proje geliştirme ve işbirliği için:
 - E-posta: [eyup.tp@hotmail.com](mailto:eyup.tp@hotmail.com)
Veri seti hakkında soru ve geri bildirimleriniz için lütfen bu repository'de bir [issue oluşturun](https://github.com/yourusername/Turkish-NLP-QQ-Dataset/issues).

---
