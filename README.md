# EBOB_EKOK-while-

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        System.out.println("Küçük sayıyı giriniz: ");
        int n1= input.nextInt();

        System.out.println("Büyük sayıyı giriniz: ");
        int n2= input.nextInt();
        int ebob =1;
        int ekok=1;

        int k=n1;
        while(k>= 1){
            if (n1%k==0 && n2%k==0){
                ebob=k;
                System.out.println(ebob);
                break;
            }else {
                k--;
            }
        }
        int i=n2;
       while (i<=(n1*n2)){
            if (i%n1==0 && i%n2==0){
                System.out.println(i);
                break;
            }else {
                i++;
            }
        }
    }
}
