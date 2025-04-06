class Main {

    public static void main(String[] args) {
        System.out.println(advice(3, 2)); // 5.0
        System.out.println(pen(3, 2)); // 1.0
        System.out.println(oleg(3, 2)); // 6.0
        System.out.println(fish(3, 2)); // 1.5
    }

    public static double advice(double a, double b) {
        return a + b;
    }

    public static double pen(double a, double b) {
        return a - b;
    }

    public static double oleg(double a, double b) {
        return a * b;
    }

    public static double fish(double a, double b) {
        if (b == 0) {
            throw new IllegalArgumentException("Деление на ноль невозможно.");
        }
        return a / b;
    }
}
