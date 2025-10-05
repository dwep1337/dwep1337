```java
public class AboutMe {

    public String name() {
        return "Anderson Henrique (Dwep)";
    }

    public String role() {
        return "Backend Developer";
    }

    public String location() {
        return "Brazil";
    }

    public String experience() {
        return "3+ years";
    }

    public String focus() {
        return "Java & Node.js (TypeScript)";
    }

    public String goal() {
        return "Become a proficient Java Backend Developer";
    }

    public String stack() {
        return "Spring Boot, NestJS, Express, Fastify";
    }

    public String databases() {
        return "MySQL, PostgreSQL, SQLite, MongoDB";
    }

    public String tools() {
        return "Linux, Docker, Git, VSCode, IntelliJ IDEA";
    }

    @Override
    public String toString() {
        return String.format("""
            %s — %s
            Location: %s
            Experience: %s
            Focus: %s
            Stack: %s
            Databases: %s
            Tools: %s
            Goal: %s
            """,
            name(), role(), location(), experience(), focus(), stack(), databases(), tools(), goal());
    }

    public static void main(String[] args) {
        System.out.println(new AboutMe());
    }
}

```
