// Problem: Usage of System.exit(0) in nested exception program. 

class Code {

    public static void main(String... code) {

        while (true) {

            System.out.println("Enter the value of n: ");

            Scanner s = new Scanner(System.in);

            int n = s.nextInt();

            try {

                System.out.println("The output is : " + 10 / n);

                System.exit(1);

            } catch (ArithmeticException e) {

                try {

                    System.out.println("Enter the index to find the character at the index: ");

                    int m =s.nextInt();

                    System.out.println("The character at the given index is: " + "abhishek".charAt(m));

                }

                catch (Exception r){

                    System.out.println("Ooopss, the exception occured is:"+ r);

                }

            }System.out.println("The task finished\n Thank You");

        }

    }

}

/*

Enter the value of n:

2

The output is : 5

 */
