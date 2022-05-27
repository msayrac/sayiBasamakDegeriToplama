# sayiBasamakDegeriToplama
import java.io.InputStream;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        int number;

        Scanner input = new Scanner(System.in);
        System.out.println("Lutfen bir sayi giriniz : ");
        number = input.nextInt();
        int basamakNumber = 0;
        int tempNumber=number;
        int basValue;
        int result=0;
        int basPow;
        while(tempNumber!=0){
            tempNumber = tempNumber/10;
            basamakNumber++;
        }
        System.out.println("kac basamaklı sayi : " + basamakNumber);
        tempNumber=number;
        while(tempNumber!=0){
            basValue=tempNumber%10;
            result=result+basValue;
            tempNumber=tempNumber/10;
        }
        System.out.println("basamak degeri : " + result);
    }
}
