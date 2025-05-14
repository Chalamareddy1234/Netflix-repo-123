import java.util.Scanner;

public class LoginPage {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String username, password;

        System.out.print("Username: ");
        username = scanner.nextLine();

        System.out.print("Password: ");
        password = scanner.nextLine();

        if (authenticate(username, password)) {
            System.out.println("Login successful!");
        } else {
            System.out.println("Login failed. Invalid username or password.");
        }
        scanner.close();
    }

    public static boolean authenticate(String username, String password) {
        // Replace with database or other authentication mechanism in a real application
        return username.equals("user") && password.equals("password");
    }
}
