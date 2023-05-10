# ÖDEV
**Dersler : Matematik , Fizik , Kimya , Türkçe , Müzik;**
* Geçme Notu : 55
* Ödev : Eğer girilen notlar 0 ve 100 aralığında değilse ortalamaya katılmasın.
```
import java.util.Scanner;

public class sinifGecme {
    public static void main(String[] args) {
        int mat,fizik,kimya,turkce,muzik;
        Scanner input = new Scanner(System.in);

        System.out.print("Matematik Notunuz : ");
        mat = input.nextInt();

        System.out.print("Fizik Notunuz : ");
        fizik = input.nextInt();

        System.out.print("Kimya Notunuz : ");
        kimya = input.nextInt();

        System.out.print("Türkçe Notunuz : ");
        turkce = input.nextInt();

        System.out.print("Müzik Notunuz : ");
        muzik = input.nextInt();


        int i=0,top=0;

        if ((mat>=0)&&(mat<=100)){
            i++;
            top = top + mat ;
        }
        if ((fizik<=100)&&(fizik>=0)){
            i = i+1;
            top = top + fizik ;
        }
        if ((kimya<=100)&&(kimya>=0)){
            i = i + 1;
            top = top + kimya ;
        }
        if ((turkce<=100)&&(turkce>=0)){
            i = i + 1 ;
            top = top + turkce;
        }
        if ((muzik<=100)&&(muzik>=0)){
            i = i + 1 ;
            top = top + muzik ;
        }
        double average = (top / i);

        if (average <55){
            System.out.println("Sınıfta Kaldınız, Seneye Tekrar Görüşmek Üzere!!");
        }else {
            System.out.println("Tebrikler Sınıfı Geçtiniz!!");
        }
        System.out.print("Ortalama Notunuz : " + average);
    }
}
```
***
# Patika Linkim :
<a href="https://academy.patika.dev/profile">PaTiKa linkim</a>
