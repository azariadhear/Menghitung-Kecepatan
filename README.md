# Menghitung-Kecepatan
package Kecepatan;
import java.util.Scanner;
public class Kecepatan {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("KALKULATOR KECEPATAN");
        double jarak, waktu, jam, menit, detik, ms, kmh, mph;
        System.out.print("Masukkan jarak (meter):");
        jarak = sc.nextDouble();
        System.out.print("Masukkan waktu tempuh (jam):");
        jam = sc.nextDouble();
        System.out.print("Masukkan waktu tempuh (menit) :");
        menit = sc.nextDouble();
        System.out.print("Masukkan waktu tempuh (detik) :");
        detik = sc.nextDouble();
        waktu = (3600*jam)+(60*menit)+detik;
        ms = jarak/waktu;
        kmh = 3.6*ms;
        mph = 2.23693629*ms;
        
        System.out.println("v (m/s) : " + ms);
        System.out.println("v (km/h) : " + kmh);
        System.out.println("v (mil/h) : " + mph);
    }
}
