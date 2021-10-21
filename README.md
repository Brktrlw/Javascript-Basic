# Temel Bilgiler

- Değişken
    
    ```jsx
    const degisken="berkay"; // Değişkenin değeri hiçbir zaman değişmez.eğer if bloklarında 
    //let ile değişken oluşturursak  o değişken if bloguna özgü olur dışarıdan ulaşamayız
    let degisken ="berkay";  // eğer if bloklarında let ile değişken oluşturursak o değişken 
    //if bloguna özgü olur dışarıdan ulaşamayız
    var degisken ="berkay";  // eğer if bloklarında var ile değişken oluşturursak ,değişkene
    //dışarıdan da ulaşırız
    console.log(typeof(degisken));
    
    var isim="berkay",soyisim="şen",yas=20; // tek satırda birden fazla değişken oluşturma
    ```
    
- Tip dönüşümleri
    
    ```jsx
    let sayi1 = Number("4"); // Değişkeni sayıya çevirir
    let sayi3 = parseInt("10"); // Değişkeni sayıya çevirir ondalıkları atar 
    let sayi4 = parseFloat("10"); // Değişkeni sayıya ondalıklı şekilde çevirir
    let sayi2 = String(10);  // Değişkeni metine çevirir
    var age=4.000000
    console.log(age.toFixed(4)) // Sonuç : 4.0000 Virgülden sonra kaç tane hane olacagını belirleriz
    ```
    
- Operatörler
    
    ```jsx
    5 ==="5" false döndürür çünkü 3 eşittir hem değer hem de tip karsılastırması yapar
    ```
    
- Date İşlemleri
    
    ```jsx
    let tarih=new Date();
    console.log(tarih.getDay()); // Ay yıl gün saniye saat vs alabiliriz.
    tarih.setMonth(5); // Gibi kendimiz tarih objesi oluşturabiliriz (ay yıl saat gün etc.)
    let tarih=new Date(2021,1,5); // Şeklinde de tarih objesi oluşturabiliriz
    let tarih=new Date("8/24/2021 14:50:10"); // Şeklinde de tarih objesi oluşturabiliriz
    ```
    
- String methodları
    
    ```jsx
    degisken.replace(/ /g,"-"); // bulduğu tüm bosluk karakterlerini - yapar (g harfi özeldir)
    degisken.search(/BeRkAy/i); // küçük büyük harf duyarlı olmadan arama yapar / /i
    var result= `merhaba ben ${isim}`; // formatlama işlemleri
    eval("isim + result"));         // Parametreyi js ifadesi gibi çalıştırıp yazdırır
    var sonuc=isim.slice(1,5);      // stringi 1. indexten baslayıp 5.indexe kadar kopyalar
    var sonuc=isim.substring(1,5);  // 1den 5e kadar olan yeri alır
    var sonuc=isim.substr(1,5);     // 1den başla 5 karakter git FARKLI
    var sonuc=isim.valueOf();       // değeri ve değişken türünü aynı şekilde kopyalar
    var sonuc=isim.indexOf("b",10); // b harfini 10.indexten itibaren arar ve bulduğu ilk indexi döndürür bulamazsa -1 döndürür
    var sonuc=isim.lastIndexOf("ber"); // ifadede "ber" kelimesini arar ve en son bulduğu indexi döndürür
    var sonuc=isim.includes("a");   // değişkende a harfi varsa true yoksa false döndürür
    var sonuc=isim.charAt(5);       // 5.indexteki karakteri döndürür
    var sonuc=isim.sub();           // alt simge yapar H2O gibi
    var sonuc=isim.sup();           // m2 (metre kare) üst karakter yapar
    var sonuc=isim. //              // fontcolor,fontsize,strike,italic,fixed gibi metotlar kullanılır
    var sonuc=isim.anchor("isim");  // a etiketine alıp name özelliğini verir
    var sonuc=isim.link("link");    // nesneye a hrefi verir 
    ```
    
- Liste Array İşlemleri
    
    ```jsx
    isimler=["ali"];
    isimler.push("berkay");   // Listenin sonuna eleman ekler
    isimler.unshift("berkay"); // listenin başına eleman ekler
    
    isimler.pop() // son elemanı siler
    isimler.shift() // ilk elemanı siler
    
    var index=isimler.indexOf("ali"); // alinin kaçıncı indexde olduğunu bulur ( 0 ) bulamazsa -1 döndürür
    isimler.sort(); // listeyi sıralar
    var birlesikListe =i simler.concat(yeniListe); // iki listeyi yan yana birleştirir
    
    ```
    
- Döngüler
    
    ### For Döngüsü
    
    ```jsx
    for(let i in liste)
    {
        console.log(i);
    }
    for(a=0;b<10;a++,b--) // arttırma ve azaltmaları virgül ile ayırabiliriz
    {
    // do something
    }
    ```
    
- Koşul
    
    ```jsx
    var a=(koşul) ? ifade1:ifade2 // ternary kosul ifadesi denir
    ```
    
    ```jsx
    var deger=5;
    switch(deger)
    {
    		case 1:                 // deger==1 ise
    		console.log("cevap 1"); // do something
    		break;
    
    		case 2:
    		console.log("cevap 2"); 
    		break;
    		
    		default:
    		console.log("default (else) çalıştı");
    }
    ```
    
    /tog
    
    /tog