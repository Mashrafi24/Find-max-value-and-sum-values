# Find-max-value-and-sum-values



    import java.util.Scanner;

    public class FileProcess {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("Enter integers (type -1 to stop):");

        int max = Integer.MIN_VALUE;

        while (true) {
            int n = sc.nextInt();
            if (n == -1) {
                break;
            }
            if (n > max) {
                max = n;
            }
        }

        if (max == Integer.MIN_VALUE) {
            System.out.println("No numbers entered");
        } else {
            long sum = (long) max * (max + 1) / 2;
            System.out.println("Max = " + max);
            System.out.println("Sum = " + sum);
        }

        sc.close();
    }
}
