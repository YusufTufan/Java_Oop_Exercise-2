# Point Sınıfı
Bu Java sınıfı, iki boyutlu uzayda bir noktayı temsil eder. Noktanın X ve Y koordinatlarına erişmek, bu koordinatları ayarlamak, noktanın orijinden uzaklığını hesaplamak ve diğer noktalara olan uzaklığı bulmak gibi işlevleri içerir.

## Kullanım
Sınıfı kullanmak için aşağıdaki adımları izleyin:

1. `Point` sınıfını projenize dahil edin.
2. Nokta oluşturmak için `Point` sınıfının yapıcılarını kullanın.
3. Noktanın özelliklerine erişmek için getter ve setter metodlarını kullanın.
4. Noktanın özelliklerini ekrana yazdırmak için `display()` metodunu kullanın.
5. Noktanın orijinden uzaklığını hesaplamak için `distanceFromOrigin()` metodunu kullanın.
6. Belirli bir koordinattaki noktaya olan uzaklığı hesaplamak için `distanceFromCoordinates(int x1, int y1)` metodunu kullanın.
7. Başka bir noktaya olan uzaklığı hesaplamak için `distanceFromPoint(Point p)` metodunu kullanın.

## Örnek

```java
public class Main {
    public static void main(String[] args) {
        // Nokta oluşturma
        Point nokta1 = new Point(3, 4);
        
        // Noktanın koordinatlarını ekrana yazdırma
        nokta1.display();
        
        // Noktanın orijinden uzaklığını hesaplama
        double uzaklik = nokta1.distanceFromOrigin();
        System.out.println("Orijinden uzaklık: " + uzaklik);
        
        // Belirli bir koordinattaki noktaya olan uzaklığı hesaplama
        double uzaklikKoordinat = nokta1.distanceFromCoordinates(5, 6);
        System.out.println("Belirli koordinattaki uzaklık: " + uzaklikKoordinat);
        
        // Başka bir noktaya olan uzaklığı hesaplama
        Point nokta2 = new Point(6, 8);
        double uzaklikNokta = nokta1.distanceFromPoint(nokta2);
        System.out.println("Başka bir noktaya olan uzaklık: " + uzaklikNokta);
    }
}
```

## Notlar
- Bu sınıf, noktaları temsil etmek için kullanılır.
- Metotlar ve alanlar aracılığıyla noktanın özelliklerine erişim sağlanır.
- Bazı metotlar, noktanın konumunu ve diğer noktalara olan uzaklığını hesaplar.
--- 

Bu README dosyası, `Point` sınıfının ne yaptığını, nasıl kullanılacağını ve hangi özelliklere sahip olduğunu açıklar. Ayrıca, kullanıcıya sınıfı kullanmak için gerekli adımları, örnek kullanımı ve dikkat edilmesi gereken notları içerir.
