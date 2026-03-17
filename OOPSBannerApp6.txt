
class Banner {

    public String[] buildO() {
        return new String[] {
                " ***** ",
                "*     *",
                "*     *",
                "*     *",
                " ***** "
        };
    }

    public String[] buildP() {
        return new String[] {
                " ***** ",
                "*     *",
                " ***** ",
                "*      ",
                "*      "
        };
    }

    public String[] buildS() {
        return new String[] {
                " ***** ",
                "*      ",
                " ***** ",
                "      *",
                " ***** "
        };
    }
}

public class Main {

    public static void main(String[] args) {

        Banner banner = new Banner();

        String[] O1 = banner.buildO();
        String[] O2 = banner.buildO(); // Reusing O
        String[] P = banner.buildP();
        String[] S = banner.buildS();

        for (int i = 0; i < O1.length; i++) {
            System.out.println(O1[i] + "   " +
                    O2[i] + "   " +
                    P[i] + "   " +
                    S[i]);
        }
    }
}