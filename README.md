# Reto_06
---
**Nota:** Los ejercicios del 1-6 se encuentran en el notebook anexo a este repositorio

---
Diagramas de flujo de los puntos 1,2,3


**Diagrama de flujo - Punto 1**

```mermaid
flowchart  TD
    A[Inicio] --> B[i = 0]
    B --> C{while i <= 100}
    C -->|Sí| D[Imprimir i y i^2]
    D --> E[i = i + 1]
    E --> C
    C -->|No| F[Fin]

```
---
**Diagrama de flujo - Punto 2**

```mermaid
flowchart TD
    A["Inicio"] --> B["Imprimir impares desde 1 hasta 999:"]
    B --> C["for i en rango(1, 1000, 2)"]
    A --> E[Imprimir pares desde 2 hasta 1000:]
    E --> F["for i en rango(2, 1001, 2)"]
    C --> D["Imprimir i"]
    F --> G["Imprimir i"]
```
---
**Diagrama de flujo - Punto 3**

```mermaid
flowchart TD
    A["Inicio"] --> B["Ingresa numero"]
    B --> C{"if num % 2 &gt; 0"}
    C -- Sí --> D["num -1"]
    D --> E["for i en rango(num, 1, -2)"]
    C -- No --> E
    E --> F["Imprimir i"]
    F --> E
    F --> G["Fin"]
```
