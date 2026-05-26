```markdown
**Title**: Seguridad Cuántica en NB-IoT: Protección de Datos contra Amenazas Cibernéticas en Comunicaciones de Exploración Profunda

**Description**: El proyecto analiza las vulnerabilidades de la criptografía clásica en redes NB-IoT frente a amenazas cuánticas (algoritmos de Shor y Grover) y propone una arquitectura híbrida de seguridad post-cuántica (PQC) adaptada a las restricciones de dispositivos de bajo consumo. La solución combina onboarding basado en ML-KEM en el plano de control con protección ligera en el plano de datos, manteniendo compatibilidad con estándares 3GPP. Se evalúa su rendimiento en escenarios de exploración profunda mediante pruebas en hardware real y simulaciones a escala, midiendo consumo energético, latencia y overhead de comunicación.

**General Objective**: Desarrollar y validar una arquitectura híbrida de seguridad post-cuántica para redes NB-IoT que proteja datos sensibles en entornos de exploración profunda contra amenazas cibernéticas cuánticas actuales y futuras.

**Specific Objectives**: 
- Analizar las vulnerabilidades de los mecanismos de seguridad actuales de NB-IoT frente a computación cuántica y el modelo harvest-now-decrypt-later.
- Diseñar una arquitectura híbrida PQC-aware que separe el plano de control y el plano de datos manteniendo compatibilidad con protocolos 3GPP.
- Implementar y evaluar el rendimiento de algoritmos seleccionados (ML-KEM-512 y ML-DSA-44) en plataformas NB-IoT reales y simuladas.
- Cuantificar los trade-offs en consumo energético, latencia y overhead de comunicación en escenarios remotos.
- Identificar limitaciones y proponer recomendaciones para la integración en estándares futuros.

**Justification**: La convergencia de la computación cuántica y el crecimiento exponencial de dispositivos NB-IoT en aplicaciones críticas (monitoreo ambiental, minería, exploración oceánica y submarina) genera un riesgo estratégico elevado. Los datos transmitidos hoy pueden ser almacenados y descifrados en el futuro, comprometiendo infraestructuras de misión crítica. Este proyecto aporta una solución práctica y compatible que facilita la transición hacia la criptografía post-cuántica, contribuyendo a la soberanía tecnológica y la protección de infraestructuras críticas.

**Methodology**: Se adopta un enfoque experimental híbrido que combina revisión del estado del arte, diseño arquitectónico, implementación en hardware (módulos Quectel BC95-G) y simulaciones a gran escala en NS-3. Se utilizan primitivas estandarizadas por NIST (ML-KEM y ML-DSA), mediciones con power profilers y análisis comparativo contra baselines clásicos bajo condiciones que emulan entornos de exploración profunda.

**Scope**: Desarrollo y validación de una arquitectura PQC híbrida para NB-IoT en escenarios remotos, con evaluación cuantitativa de rendimiento y seguridad (máx. 100 caracteres).

**Activities**: 
1. Revisión bibliográfica y análisis de amenazas cuánticas.
2. Diseño de la arquitectura híbrida y definición de protocolos.
3. Implementación en plataforma hardware y entorno de simulación.
4. Ejecución de pruebas de rendimiento y análisis de resultados.
5. Redacción del artículo y documentación de limitaciones y trabajos futuros.

**Resources**: 
- Hardware: Módulos NB-IoT Quectel BC95-G, eNodeB emulado (srsRAN), power profiler Keysight.
- Software: NS-3, librerías PQC (liboqs), srsRAN, herramientas de análisis de consumo energético.
- Datos: Benchmarks de algoritmos PQC y trazas de tráfico en entornos remotos.

**Limitations**: 
- Dependencia de hardware comercial con restricciones de memoria y procesamiento.
- Penalización energética (aprox. 18% en vida útil de batería).
- Validación limitada en entornos de campo reales a gran escala.
- Madurez actual de las implementaciones PQC en dispositivos de ultra-bajo consumo.
```

**Nota**: Este registro está listo para ingresar directamente en una base de datos de proyectos de investigación.