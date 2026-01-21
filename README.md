package mariaveronica;

import java.util.Scanner;

/**
 *
 * @author ADMIN
 */
public class MariaVeronica {

    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        System.out.println("Student Information");
        System.out.println("-------------------");
        Student student1 = new Student();
        System.out.print("Enter name: ");
        student1.name = input.nextLine();
        System.out.print("Enter age: ");
        student1.age = input.nextInt();
        input.nextLine(); // consume newline
        System.out.print("Enter course: ");
        student1.course = input.nextLine();

        System.out.println();

        Student student2 = new Student();
        System.out.print("Enter name: ");
        student2.name = input.nextLine();
        System.out.print("Enter age: ");
        student2.age = input.nextInt();
        input.nextLine(); // consume newline
        System.out.print("Enter course: ");
        student2.course = input.nextLine();

        System.out.println("\nStudent Details");
        System.out.println("-------------------");

        student1.displayInfo();
        student2.displayInfo();

        input.close();
    }
}

 class Student {

    String name;
    int age;
    String course;

    void displayInfo() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Course: " + course);
        System.out.println();
    }
}
