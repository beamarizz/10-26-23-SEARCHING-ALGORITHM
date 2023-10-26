import java.util.HashMap;
import java.util.Scanner;

public class HashTableExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        HashMap<Integer, String>[] hashTable = new HashMap[10];

        for (int i = 0; i < 10; i++) {
            hashTable[i] = new HashMap<>();
        }

        while (true) {
            System.out.print("Enter a key (integer) or -1 to exit: ");
            int key = scanner.nextInt();

            if (key == -1) {
                break;
            }

            System.out.print("Enter a value (string): ");
            String value = scanner.next();

            int index = key % 10; // Use key % 10 to determine the index based on the remainder
            hashTable[index].put(key, value);
        }

        System.out.println("Hash Table Contents:");

        for (int i = 0; i < 10; i++) {
            System.out.println("Index " + i + ": " + hashTable[i]);
        }
    }
}