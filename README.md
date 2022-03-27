# Min-Max-Bulma
Patika.dev > Java101 > Döngüler > Ödev1 - Girilen Sayılardan Min ve Max Değerleri Bulma 

## Java ile klavyeden girilen N tane sayma sayısından en büyük ve en küçük sayıları bulan ve bu sayıları ekrana yazan programı yazın.


      import java.util.*;

      public class min_max_bulma {

        public static void main(String[] args) {

          Scanner sc = new Scanner(System.in);

          int temp,adet,max=0,min=0;

          System.out.println("Kaç adet sayı gireceksiniz:");
          adet = sc.nextInt();

          for(int i=1; i<=adet; i++) {

            System.out.println("Lütfen " + i + ". sayıyı giriniz:");
            temp = sc.nextInt();

            if(temp < min)	
              min = temp;

            if(temp > max)
              max = temp;
          }

          System.out.println("En büyük sayı: " + max);
          System.out.println("En küçük sayı: " + min);

        }
      }
