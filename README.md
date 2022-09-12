# enBuyukEnKucukSayi


import java.util.Scanner;
class Main {
    public static void main(String[] args) {
        Scanner inp = new Scanner(System.in);
        int n1, min = 1, b;
        int n = 1, max = 1;

        System.out.println("Kaç tane sayı gireceksiniz");
        n = inp.nextInt();
        for (int i = 1; i <= n; i++) {
            System.out.print(i + ". Sayıyı Giriniz:");
            n1 = inp.nextInt();
            if (i == 1) {
                min = n1;
                max = n1;
            }
            if (n1 > max) {
                max = n1;
            }if (n1 <min) {
                min = n1;
            }
        }
        System.out.println("En Büyük Sayı: "+max);
        System.out.println("En Küçük Sayı: "+min);
    }
}
