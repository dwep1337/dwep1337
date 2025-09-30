```java
import java.util.List;
import java.util.Map;

public class AboutMe {

    public String getName() {
        return "Anderson Henrique (Dwep)";
    }

    public String getRole() {
        return "Backend Developer";
    }

    public String getLocation() {
        return "Brazil";
    }

    public String getEducation() {
        return "Undergraduate in Analysis and Systems Development (ADS)";
    }

    public String getGoal() {
        return "Become a proficient Java Backend Developer and contribute to open-source projects";
    }

    public String getYearsOfExperience() {
        return "3+ years";
    }

    public Map<String, List<String>> getTechnicalSkills() {
        return Map.of(
            "Languages", List.of("Java", "TypeScript", "JavaScript", "SQL"),
            "Frameworks", List.of("Spring Boot", "NestJS", "Node.js", "Hibernate"),
            "Databases", List.of("MySQL", "PostgreSQL", "MongoDB"),
            "DevOps & Cloud", List.of("Docker", "RabbitMQ", "AWS"),
            "Other", List.of("Git", "REST APIs", "Microservices", "OOP")
        );
    }

    public List<String> getTools() {
        return List.of("IntelliJ IDEA", "VSCode", "Postman", "Docker", "Git/GitHub", "RabbitMQ", "Linux");
    }

    public Map<String, List<String>> getInterests() {
        return Map.of(
            "Professional", List.of("Backend Architecture", "Performance Optimization", "Clean Code"),
            "Personal", List.of("Coding", "Gaming", "Linux distros", "Open-source")
        );
    }

    public Map<String, String> getContacts() {
        return Map.of(
            "Email", "dwepdeveloper@outlook.com",
            "LinkedIn", "https://www.linkedin.com/in/anderson-h/"
        );
    }

    public List<String> getCurrentFocus() {
        return List.of("Deepening Spring Boot", "Improving system design");
    }

    @Override
    public String toString() {
        return String.format("""
            %s - %s (Backend Developer)
            Location: %s
            Education: %s
            Goal: %s
            """, 
            getName(), getRole(), getLocation(), getEducation(), getGoal());
    }
}

```
