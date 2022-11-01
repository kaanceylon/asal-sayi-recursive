# asal-sayi-recursive
import javax.swing.plaf.synth.SynthLookAndFeel;
import java.awt.*;
import java.sql.PreparedStatement;
import java.util.Scanner;

public class Main {

    static boolean asalsayi(int sayi){
        int sayac =0;
        for (int i=2; i < sayi; i++){
            if (sayi % i == 0){
                sayac ++;
            }
        }
        if (sayac == 0){
            return true;
        }
        else{
            return false;
        }
    }
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.print("Bir sayi giriniz: ");
        int sayi = input.nextInt();
        if (asalsayi(sayi)){
            System.out.print("Bir asal sayidir.");
        }
        else{
            System.out.print("Bir asal sayi değildir.");
        }

    }
}
































