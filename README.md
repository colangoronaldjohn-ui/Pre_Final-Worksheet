public class FactorialTrace {

    public static int factorial(int n) {
        System.out.println("Call: factorial(" + n + ")");

        if (n == 0) {
            System.out.println("Return: factorial(0) = 1");
            return 1;
        }

        int result = n * factorial(n - 1);
        System.out.println("Return: factorial(" + n + ") = " + result);
        return result;
    }

    public static void main(String[] args) {
        System.out.println("Final Answer: " + factorial(4));
    }
}