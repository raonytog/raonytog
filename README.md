```java
class Ray {
    private String name;
    private String mainLanguage;
    private String secondLanguage;
    private int age;

    public Ray() {
        this.name = "Ray";
        this.mainLanguage = "pt-BR";
        this.secondLanguage = "en-US";
        this.age = 22;
    }

    public void HeyThere() {
        System.out.println("\n-======================@==========================-");
        System.out.println("Hi! I'm a Comp.Sci student in the seventh semester at UFES.");
        System.out.println("I have experience a few moderns programming languages like C/C++, Python, Java, Swift, TypeScript");
        System.out.println("Also, some tecnologies like React, Pandas, SpringBoot, Bootstrap, Thymeleaf, Nest.JS, Next.JS, Postgree");
        System.out.println("-======================@==========================-\n");
      }

    public void GoodBye() {
        System.out.println("\n-======================@==========================-");
        System.out.println("Thanks for visiting my profile!");
        System.out.println("See you soon, my dear! :) ");
        System.out.println("-======================@==========================-\n");
    }
}

public class Main {
    public static void main(String[] args) {
        Ray myself = new Ray();
        myself.HeyThere();
        myself.GoodBye();
    }
}

```




