# Java-Management-System
interface Developer {
    void code();
}

interface Designer {
    void design();
}

class Techland implements Developer, Designer {

    @Override
    public void code() {
        System.out.println("Developer is writing code.");
    }

    @Override
    public void design() {
        System.out.println("Designer is creating design.");
    }
}

public class EmployeeManagement {
    public static void main(String[] args) {

        Techland employee = new Techland();

        employee.code();
        employee.design();
    }
}
