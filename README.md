# Dik-ucgende-Hipotenus
patika.dev Dik Üçgende Hipotenüs


import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        //Değişkenleri Oluştur.
        double a, b, hipotenus, u, cevre, alan;

        //kullanıcıdan Verileri Al
        Scanner girdi = new Scanner(System.in);
        System.out.print("1. Kenar Ölçüsünü Girin :");
        a = girdi.nextInt();
        System.out.print("2. Kenar Ölçüsünü Girin :");
        b = girdi.nextInt();

        hipotenus = Math.sqrt((a*a) + (b*b));
        System.out.println("Hipotenüs :" + hipotenus);

        u = (a+b+hipotenus)/2;
        cevre = 2 * u;
        alan = Math.sqrt(u * (u-a) * (u-b) * (u-hipotenus));

        System.out.println("Üçgenin Alanı :" + alan);


    }
}
