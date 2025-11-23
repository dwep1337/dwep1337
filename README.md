```typescript
type TechStack = readonly string[];

interface IAboutMe {
  name: string;
  role: string;
  focus: string;
  experience: string;
  location: string;
  stack: TechStack;
  show(): string;
}

class AboutMe implements IAboutMe {
  public readonly name = "Anderson Henrique (Dwep)";
  public readonly role = "Backend Developer";
  public readonly focus = "TypeScript, Java, PHP";
  public readonly experience = "3+ years";
  public readonly location = "Brazil";

  public readonly stack: TechStack = [
    "Node.js (NestJS, Express, Fastify)",
    "Java (Spring Boot)",
    "PHP"
  ];

  get mainStack(): string {
    return this.stack[0];
  }

  public show(): string {
    return `
        ${this.name} — ${this.role}
        Focus: ${this.focus}
        Experience: ${this.experience}
        Location: ${this.location}
        Stack: ${this.stack.join(", ")}
        Main Stack: ${this.mainStack}
    `;
  }
}

console.log(new AboutMe().show());
```
