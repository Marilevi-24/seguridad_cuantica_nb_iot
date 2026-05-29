## FASE 1: Mapeo de Entidades (Análisis)

Al analizar el fragmento de LaTeX proporcionado para `fig2.png`, se identifican las siguientes entidades, relaciones y niveles de abstracción:

* **Entidad Central (Raíz):** Taxonomía de Criptografía Post-Cuántica (PQC) orientada a entornos restringidos.
* **Familias Tecnológicas (Ramas Principales):** Basada en retículos (*Lattices*), basada en códigos (*Codes*), multivariable (*Multivariate*) y basada en funciones hash (*Hash-based*). *(Nota: Isogenias no se mencionan en este texto de 2026 debido a la depreciación de esquemas como SIKE tras quiebres criptográficos recientes, un detalle de precisión cronológica sutil).*
* **Instancias de Algoritmos Específicos (Nodos NIST):** ML-KEM (Kyber), ML-DSA (Dilithium), FN-DSA (Falcon) y ML-KEM-512.
* **Atributo de Calificación (Relaciones de Idoneidad):** Nivel de *Suitability* (Adecuación) para el stack 3GPP de NB-IoT en exploración profunda (Alta/Recomendada vs. Media por overhead energético/computacional).
* **Nivel de Abstracción:** Diagrama taxonómico estructurado (árbol de decisión/clasificación técnica) con codificación de colores para representar restricciones de hardware de manera analítica.

---

## FASE 2: Auditoría y Reporte de Hallazgos Críticos

### 1. Contraste de Coherencia

El prompt base propone un mapa mental genérico de PQC que incluye familias que el texto técnico no prioriza (como *Isogeny-based*). Además, el prompt base hereda la restricción de "sin texto incrustado real", lo cual contradice directamente la necesidad de la figura (`fig2.png`), cuyo epígrafe exige explícitamente mostrar la taxonomía con énfasis en la idoneidad para NB-IoT. Sin texto real, el diagrama pierde toda validez científica para el estándar IEEE.

### 2. LISTA DE DISCREPANCIAS (Explícita)

* **Ausencia de los Estándares Oficiales NIST:** El prompt base menciona nombres antiguos (Kyber, Dilithium). El LaTeX exige la nomenclatura oficial estandarizada: **ML-KEM, ML-DSA, FN-DSA y ML-KEM-512**.
* **Falta de la Métrica de Idoneidad (Suitability):** El prompt base solo tiñe de azul la rama de *Lattices*. El LaTeX (Tabla 2) exige diferenciar los niveles de idoneidad internos de dicha rama (ej. ML-KEM-512 es "Recomendada", mientras que ML-DSA posee un "Overhead elevado / Adecuación Media").
* **Inclusión de familias obsoletas/no mencionadas:** Se debe eliminar la rama de isogenias para mantener co-orientación estricta con el texto provisto.

### 3. Control de Estilo

* **Estándar:** Formato IEEE de diagramas vectoriales planos de alta densidad de información.
* **Paleta de Colores:** Azul Cobalto (`#0047AB`) exclusivo para soluciones viables/recomendadas en NB-IoT; Gris Técnico (`#4A4A4A`) para alternativas con limitaciones u overhead prohibitivo; Negro para líneas conectoras y texto tipográfico formal (Sans-Serif tipo Helvetica/Arial).

---

## FASE 3: Explicación y Justificación de Pre-ejecución

### 1. Disposición Espacial

* **Raíz Izquierda / Superior:** Nodo principal cuadrado: **"Taxonomía PQC (Restricciones NB-IoT)"**.
* **Bloques Secundarios (División por Familias):** Cuatro ramas limpias y ortogonales. La rama **"Basada en Retículos (Lattice-Based)"** se posiciona en la parte superior con mayor peso visual. Las ramas *Codes, Multivariate y Hash-based* se agrupan debajo en Gris Técnico.
* **Nodos Terminales (Hojas de Algoritmos):** Bajo la rama de Lattices, se estructuran sub-bloques específicos conectados por líneas continuas:
* `ML-KEM-512` y `ML-KEM (Kyber)` encuadrados en **Azul Cobalto** con la etiqueta incrustada *"Alta Adecuación / Recomendado"*.
* `ML-DSA (Dilithium)` y `FN-DSA` encuadrados en un degradado grisáceo o línea discontinua con la etiqueta *"Adecuación Media (Overhead Elevado)"*.



### 2. Justificación Técnica

La separación visual dentro de la familia *Lattice-based* es fundamental. Como experto aeroespacial, sé que un ingeniero de sistemas NB-IoT no puede implementar ML-DSA para firmas ligeras en un sensor bajo el agua sin evaluar el overhead de energía. La composición propuesta permite mapear la teoría matemática abstracta directamente con la viabilidad ingenieril en el plano físico de la exploración profunda.

### 3. ADVERTENCIAS PARA EL USUARIO

> ⚠️ **Puntos Críticos de Validación:**
> 1. El prompt final forzará la generación de texto técnico real en inglés científico (estándar de publicación). Existe el riesgo de que el motor de renderizado cometa micro-erratas tipográficas en caracteres pequeños.
> 2. Se omitirán íconos complejos (como escudos decorativos o chips tridimensionales) para priorizar la legibilidad pura del mapa taxonómico exigido por el formato IEEE.
> 
> 

---

## FASE 4: Ejecución Silenciosa

He diseñado y optimizado el prompt para la arquitectura de visualización requerida, subsanando todas las deficiencias criptográficas del prompt base.

Por favor, **confirma con un "Proceder"** para realizar la generación del diagrama técnico.