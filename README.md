# s-n-fgecme
package patika;
import java.util.Scanner;


public class kosulsınıfgecme {

	public static void main(String[] args) {
		int mat,fizik,turkce,kimya,muzik,toplam,dersSayisi=5;
		double ortalama;
	 Scanner inp = new Scanner(System.in);
	 System.out.println("Matematik notunuzu giriniz:");
	 mat = inp.nextInt();
	 
	 System.out.println("Fizik notunuzu giriniz:");
	 fizik = inp.nextInt();
	 
	 System.out.println("Türkçe notunuzu giriniz:");
	 turkce = inp.nextInt();
	 
	 System.out.println("Kimya notunuzu giriniz:");
	 kimya = inp.nextInt();
	 
	 System.out.println("Muzik notunuzu giriniz:");
	 muzik = inp.nextInt();
	  if (mat< 0 || mat > 100) {
          mat = 0;
          dersSayisi--;
      }

      if (fizik < 0 || fizik > 100) {
          fizik = 0;
          dersSayisi--;
      }

      if (turkce < 0 || turkce > 100) {
          turkce = 0;
          dersSayisi--;
      }

      if (kimya < 0 || kimya > 100) {
          kimya = 0;
          dersSayisi--;
      }

      if (muzik < 0 || muzik > 100) {
          muzik = 0;
          dersSayisi--;
      }
	
	 toplam = (mat +fizik+turkce+kimya+muzik);
	 
	 ortalama = (toplam/6);
	 
	 System.out.println("Ortalamanız =" +ortalama);
	 
	 if (ortalama<55) {
		System.out.println("Üzgünüm,sınıfta kaldınız.");
	} else {
		System.out.println("Tebrikler,sınıfı geçtiniz.");
 
	}
	 

	}

}
