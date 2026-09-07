<h1 align="center">Devops-Learning-with-Yuvraj</h1>

A collection of hands-on exercises focused on learning Cloud Fundamentals and DevOps scripting.

> **Learn the fundamentals → Automate → Containerize → Deploy → Monitor → Build real projects**

### What Each Technology Teaches

- **Linux** teaches you the server.
- **Networking** teaches you how servers communicate.
- **Git** teaches you version control.
- **Bash** teaches you automation.
- **YAML** teaches you configuration.
- **Docker** teaches you containers.
- **Docker Compose** teaches you multi-container applications.
- **Jenkins / GitHub Actions** teach you CI/CD.
- **Kubernetes** teaches you container orchestration.
- **Helm** makes Kubernetes deployments easier.
- **GitOps + Argo CD** automate Kubernetes deployments from Git.
- **Prometheus + Grafana** teach monitoring and observability.
- **Terraform** teaches Infrastructure as Code.
- **AWS** teaches cloud infrastructure.
- **Projects** bring everything together.

# DevOps Learning Roadmap

```mermaid
flowchart TD

    A["DevOps Learning Roadmap"]

    B["1. Linux"]
    C["2. Networking"]
    D["3. Git"]
    E["4. Bash Scripting"]
    F["5. YAML"]
    G["6. Docker"]
    H["7. Docker Compose"]
    I["8. CI/CD"]

    J["9. Jenkins"]
    K["10. GitHub Actions"]

    L["11. Kubernetes"]
    M["12. Helm"]
    N["13. GitOps"]
    O["14. Argo CD"]
    P["15. Prometheus"]
    Q["16. Grafana"]
    R["17. Terraform"]
    S["18. Cloud / AWS"]
    T["19. Advanced DevOps Projects"]

    A --> B
    B --> C
    C --> D
    D --> E
    E --> F
    F --> G
    G --> H
    H --> I

    I --> J
    I --> K

    J --> L
    K --> L

    L --> M
    M --> N
    N --> O
    O --> P
    P --> Q
    Q --> R
    R --> S
    S --> T

    classDef roadmap fill:#06345B,stroke:#B9D9F5,color:#A9D2F5,stroke-width:1px;

    class A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T roadmap;
```
