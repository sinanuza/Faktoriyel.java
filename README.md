# Faktoriyel.java
www.patika.dev Faktoriyel kavrami



       import java.util.Scanner;

        public class Faktoriyel {
        public static void main(String[] args) {
        int i,n,r,total1,total2,total3,sonuc;
        System.out.println("C(n,r) icin n sayisini giriniz:");
        Scanner input=new Scanner(System.in);
        n=input.nextInt();
        System.out.println("C(n,r) icin r sayisini giriniz");
        r=input.nextInt();
        total1=1;
        total2=1;
        total3=1;
        for (i=1;i<=n;i++){
            total1=total1*i;
        }
        for (int j=1;j<=r;j++){
            total2=total2*j;
        }
        for (int k=1;k<=(n-r);k++){
            total3=total3*k;
        }
        sonuc=total1/(total2*total3);
        System.out.println("Sonucunuz:"+sonuc);
    }
}
