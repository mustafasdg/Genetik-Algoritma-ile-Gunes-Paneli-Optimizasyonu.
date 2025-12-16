# Genetik-Algoritma-ile-Gunes-Paneli-Optimizasyonu

## Proje Amacı

Bu projede, bir belediyeye ait güneş enerjisi sistemlerinde kullanılacak panellerin eğim açısı (x₁) ve yön sapması (x₂) değerleri, verilen kısıtlar altında maksimum enerji verimi sağlayacak şekilde optimize edilmiştir.

Optimizasyon problemi, sezgisel bir yöntem olan Genetik Algoritma kullanılarak çözülmüştür.

---

## Senaryo Bilgisi

Bu çalışma, ders kapsamında verilen senaryolardan "Güneş Paneli Yerleşiminde Optimum Eğim ve Yön" senaryosuna dayanmaktadır. Senaryo, öğrenci numarasının son hanesine uygun olarak seçilmiştir.

---

## Matematiksel Model

### Amaç Fonksiyonu

Amaç, aşağıdaki fonksiyonun maksimize edilmesidir:

y = 6x₁ + 4x₂ − 0.1x₁²

* x₁: Panel eğim açısı (10° – 45°)
* x₂: Güney yönüne göre sapma (0° – 90°)

### Kısıtlar

* x₁ + 0.5x₂ ≤ 60
* x₂ ≥ 15

Bu kısıtlar, panel kurulumunda karşılaşılan fiziksel sınırlamaları temsil etmektedir. Genetik algoritma yalnızca bu kısıtları sağlayan çözümleri kabul etmektedir.

---

## Kullanılan Yöntem: Genetik Algoritma

Projede klasik bir genetik algoritma yapısı uygulanmıştır. Algoritma aşağıdaki adımlardan oluşmaktadır:

1. Birey Tanımı
   Her birey, [x₁, x₂] şeklinde iki genli bir çözümü temsil eder.

2. Başlangıç Popülasyonu
   Belirlenen aralıklar ve kısıtlar dahilinde rastgele bireyler oluşturulmuştur.

3. Uygunluk (Fitness) Fonksiyonu
   Fitness fonksiyonu, her bireyin enerji verimini hesaplamaktadır. Algoritma bu değeri maksimize etmeyi amaçlar.

4. Seçilim Mekanizması – Rulet Seçimi
   Popülasyondan rastgele seçilen bireyler arasından uygunluk değeri en yüksek olan birey ebeveyn olarak seçilmektedir. Bu yöntem, genetik çeşitliliği korurken seçilim baskısını da sağlamaktadır.

5. Çaprazlama (Crossover)
   Ebeveyn bireylerin genleri rastgele oranlarda birleştirilerek yeni bireyler üretilmektedir.

6. Mutasyon
   Düşük oranlı mutasyon işlemi ile bireylerin genlerinde küçük rastgele değişiklikler yapılmaktadır. Bu işlem, algoritmanın yerel maksimumlara sıkışmasını engellemektedir.

7. Genetik Döngü
   Seçilim, çaprazlama ve mutasyon adımları belirlenen nesil sayısı boyunca tekrar edilmektedir.

---

## Sonuçlar ve Analiz

Nesiller boyunca en iyi uygunluk (fitness) değerlerinin değişimi grafikler ile gösterilmiştir. Son nesilde elde edilen en iyi bireyin x₁, x₂ ve fitness değerleri yazdırılmış ve sonuçlar yorumlanmıştır.

Elde edilen bulgular, genetik algoritmanın belirli bir noktadan sonra yakınsadığını ve kararlı bir çözüm ürettiğini göstermektedir.

---

## Akademik Dürüstlük

Bu çalışma bireysel olarak gerçekleştirilmiştir. Kodların tamamı öğrenci tarafından yazılmıştır. Hazır notebook veya doğrudan kopyalanmış içerik kullanılmamıştır.

---

## Öğrenci Bilgileri

Ad Soyad: Mustafa Yıldız
Okul Numarası: 2212729001
GitHub Repo: [https://github.com/mustafasdg/Genetik-Algoritma-ile-Gunes-Paneli-Optimizasyonu.](https://github.com/mustafasdg/Genetik-Algoritma-ile-Gunes-Paneli-Optimizasyonu.)

## Kurulum ve Çalıştırma

1 - .ipynb dosyasını Google Colab veya Jupyter Notebook ile açın.

2 - Tüm hücreleri sırasıyla çalıştırın.

3 - Sonuç grafiği en altta görüntülenecektir.



