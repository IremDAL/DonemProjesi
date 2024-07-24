# DonemProjesi
DogalDilIsleme

İlk önce bir veri seti oluşturduk. Bu veri setini twitterdan çekerek oluşturduk. Amacımız verdiğimiz tweeti algoritmalarla öğreterek hangi tweetin hangi ünlüye ait olduğunu bulmaktı.3 ünlü kişiden teker teker 1000 tane tweet çektik. Bu ünlülerimiz tarih alanından İlber Ortaylı, İki tanesi de siyaset alanından Recep Tayyip Erdoğan ve Ekrem İmamoğlu oldu. Tarih ve siyaset ile karşılaştırdık ve ekstra olarak iki siyasetçi içinde karşılaştırma yapalım algoritmalarımız nasıl çalışıyor bakmak istedik bu yüzden de iki aynı daldan kişi ekledik. Algoritma olarak TF-IDF Vectorizer ve Bayes Modelini kullandık. Stop wordsler ile ve re sub ile veri setini temizleyip clean adında bir yeni sütun ekledik. Sonrasında bu veri setine eğitim için labeller sütununu ekledik. İlber Ortaylı 0, Recep Tayyip Erdoğan 1, Ekrem İmamoğlu 2 olacak şekilde. Sonrasında modelimizi X_train ve y_train ile eğittik ve sonucumuzu test etmek için toplamda 3 tweet verdik ve bu tweetler 1000 tweetten sonraki tweetlerdi. Güzel sonuçlar elde ettik. Veri setimizi ilk başta 1500 yapmıştık veri setini 3000'e çekince modelimiz daha iyi çalıştı. Bir ek özellik daha ekledik projemize son hafta kullandığımız index.html ve model-server.py ile bir html sayfası oluşturup bu tweetleri internet üzerinden denedik algoritmalarımızı .pkl şeklinde makinemize verdik ve tahminleri kim kimin tweeti olduğu şekilde açıklayan bir html yaptık burada da güzel sonuçlar elde ettik. Fotoğrafları ekledik.
