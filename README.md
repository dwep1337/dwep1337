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

    public String getPronouns() {
        return "he/him";
    }

    public String getEducation() {
        return "Undergraduate Student in Analysis and Systems Development (ADS)";
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
            "DevOps & Cloud", List.of("Docker", "RabbitMQ", "AWS (Learning)"),
            "Other", List.of("Git", "REST APIs", "Microservices", "OOP")
        );
    }

    public List<String> getTools() {
        return List.of(
            "IntelliJ IDEA",
            "VSCode",
            "Postman",
            "Docker",
            "Git/GitHub",
            "RabbitMQ",
            "Linux (Manjaro, Ubuntu, Fedora)"
        );
    }

    public Map<String, List<String>> getInterests() {
        return Map.of(
            "Professional Interests", List.of(
                "Backend Architecture",
                "Performance Optimization",
                "Clean Code",
                "Design Patterns"
            ),
            "Personal Hobbies", List.of(
                "Coding personal projects",
                "Gaming",
                "Learning new technologies",
                "Exploring Linux distros",
                "Open-source contributions"
            )
        );
    }

    public Map<String, String> getContacts() {
        return Map.of(
            "Email", "dwepdeveloper@outlook.com",
            "LinkedIn", "https://www.linkedin.com/in/anderson-h/"
        );
    }

    public List<String> getCurrentFocus() {
        return List.of(
            "Deepening Spring Boot knowledge",
            "Improving system design skills"
        );
    }

    @Override
    public String toString() {
        return String.format("""
            About %s:
            Role: %s
            Location: %s
            Education: %s
            Goal: %s
            """, 
            getName(), getRole(), getLocation(), getEducation(), getGoal());
    }
}
```
