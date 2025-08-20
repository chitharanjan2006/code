
class Person {
    String name;
    int age;

    
    Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    void displayInfo() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}


class Student extends Person {
    String course;

    
    Student(String name, int age, String course) {
        super(name, age);
        this.course = course;
    }

    void displayStudent() {
        displayInfo(); // calling parent method
        System.out.println("Course: " + course);
    }
}

public class InheritanceExample {
    public static void main(String[] args) {
        
        Student s1 = new Student("Rahul", 20, "Computer Science");
        
        
        s1.displayStudent();
    }
}
