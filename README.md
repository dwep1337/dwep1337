```typescript
type TechStack = string[];

interface IAboutMe {
  name: string;
  role: string;
  focus: string;
  experience: string;
  location: string;
  stack: TechStack;
  toString(): string;
}

class AboutMe implements IAboutMe {
  name = "Anderson Henrique (Dwep)";
  role = "Backend Developer";
  focus = "TypeScript, Java, PHP";
  experience = "3+ years";
  location = "Brazil";

  stack: TechStack = [
    "Node.js (NestJS, Express, Fastify)",
    "Java (Spring Boot)",
    "PHP"
  ];

  get mainStack(): string {
    return this.stack[0];
  }

  toString(): string {
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

console.log(new AboutMe().toString());
```
