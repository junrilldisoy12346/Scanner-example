import java.util.Scanner;

public class EncodingExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter a message to encode: ");
        String message = scanner.nextLine();

        System.out.println("Encoded message: " + encodeMessage(message));
    }

    public static String encodeMessage(String message) {
        // Define your encoding logic here.
        // This is a simple example; you can replace it with your desired encoding algorithm.
        StringBuilder encodedMessage = new StringBuilder();
        for (char c : message.toCharArray()) {
            encodedMessage.append((char) (c + 1));
        }

        return encodedMessage.toString();
    }
}
