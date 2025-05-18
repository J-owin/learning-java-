import java.util.Scanner;
public class ee{
    public static void main(String[] args){
        Scanner scanner = new Scanner(System.in);
        double principal;
        double rate;
        int timesCompounded;
        int years;
        double amt;
        System.out.print("enter the principal amount :");
        principal = scanner.nextDouble();
        System.out.print("Enter the rate in percentage :");
        rate = scanner.nextDouble() /100;
        System.out.print("Enter the times compounded per year");
        timesCompounded = scanner.nextInt();
        System.out.print("enter years: ");
        years = scanner.nextInt();
        amt = principal * Math.pow(1+rate/timesCompounded , timesCompounded*years   );
        System.out.print("The final amount is :" + amt  );

        scanner.close();
    }
}
