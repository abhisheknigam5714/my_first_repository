# my_first_repository
new repo.
import java.util.Scanner;

public class LinearSearch {
    public LinearSearch() {
    }

    public static int LinearSearch(int[] number, int key) {
        for(int i = 0; i < number.length; ++i) {
            if (number[i] == key) {
                return i;
            }
        }

        return -1;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println(" enter the size of the array");
        int n = sc.nextInt();
        System.out.println(" enter the elements");
        int[] number = new int[n];

        int m;
        for(m = 0; m < number.length; ++m) {
            number[m] = sc.nextInt();
        }

        System.out.println(" enter the key");
        m = sc.nextInt();
        int index = LinearSearch(number, m);
        if (index == -1) {
            System.out.println(" element is not found");
        } else {
            System.out.println(" the index of the element: " + index);
        }

    }
}
