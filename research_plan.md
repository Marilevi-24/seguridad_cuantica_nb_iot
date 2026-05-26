```json
{
  "titulo": "Seguridad Cuántica en NB-IoT: Protección de Datos contra Amenazas Cibernéticas en Comunicaciones de Exploración Profunda",
  "folder_name": "seguridad_cuantica_nb_iot",
  "abstract_preliminar": "La convergencia de la computación cuántica y las redes Narrowband IoT (NB-IoT) presenta desafíos significativos para la ciberseguridad en entornos de exploración profunda, donde los dispositivos de bajo consumo transmiten datos sensibles en entornos remotos y hostiles. Este artículo analiza las vulnerabilidades de los esquemas criptográficos clásicos frente a algoritmos cuánticos como Shor y Grover, y propone un marco de seguridad cuántica basado en criptografía post-cuántica (PQC) y distribución de claves cuánticas (QKD) adaptada a las restricciones de NB-IoT. Se evalúa el estado del arte en implementaciones PQC para dispositivos restringidos, se presenta una arquitectura híbrida PQC-aware para onboarding en plano de control y protección ligera en plano de datos, y se analizan métricas de rendimiento como latencia, consumo energético y overhead de comunicación. Los resultados demuestran viabilidad práctica con optimizaciones selectivas, manteniendo compatibilidad con estándares 3GPP mientras se logra resistencia cuántica. Se discuten implicaciones para aplicaciones críticas como monitoreo ambiental y exploración industrial.",
  "secciones": [
    {
      "nro": 1,
      "titulo_seccion": "Introducción",
      "objetivos": ["Contextualizar las amenazas cuánticas a NB-IoT", "Establecer motivación para seguridad en exploración profunda", "Definir objetivos y alcance del trabajo"],
      "subsecciones": ["1.1 Motivación y Problema de Investigación", "1.2 Contribuciones Principales", "1.3 Estructura del Artículo"],
      "insumos": ["Figura 1: Arquitectura NB-IoT", "Tabla 1: Comparación amenazas clásicas vs cuánticas"],
      "llaves_bibtex": ["Liu2024_PQC_IoT", "Althobaiti2021_QuantumResistant"]
    },
    {
      "nro": 2,
      "titulo_seccion": "Antecedentes y Estado del Arte",
      "objetivos": ["Revisar fundamentos de NB-IoT y su seguridad actual", "Analizar amenazas cuánticas", "Evaluar soluciones PQC existentes"],
      "subsecciones": ["2.1 NB-IoT: Características y Vulnerabilidades", "2.2 Amenazas Cuánticas a Criptografía Clásica", "2.3 Criptografía Post-Cuántica para IoT"],
      "insumos": ["Tabla 2: Algoritmos PQC NIST", "Figura 2: Taxonomía PQC"],
      "llaves_bibtex": ["Liu2024_PQC_IoT", "Althobaiti2020_Cybersecurity", "Do2026_PQCAware"]
    },
    {
      "nro": 3,
      "titulo_seccion": "Amenazas Cibernéticas en Comunicaciones de Exploración Profunda",
      "objetivos": ["Identificar vectores de ataque específicos en NB-IoT profundo", "Evaluar impacto de computación cuántica"],
      "subsecciones": ["3.1 Escenarios de Despliegue Remoto", "3.2 Ataques de Eavesdropping y Harvest-Now-Decrypt-Later", "3.3 Limitaciones de Recursos en Entornos Hostiles"],
      "insumos": ["Tabla 3: Análisis de riesgos"],
      "llaves_bibtex": ["Althobaiti2021_QuantumResistant", "Liu2024_PQC_IoT"]
    },
    {
      "nro": 4,
      "titulo_seccion": "Propuesta de Arquitectura de Seguridad Cuántica",
      "objetivos": ["Diseñar framework híbrido PQC-QKD", "Adaptar a restricciones NB-IoT"],
      "subsecciones": ["4.1 Onboarding Post-Cuántico en Plano de Control", "4.2 Protección Ligera en Plano de Datos", "4.3 Integración con Protocolos 3GPP"],
      "insumos": ["Figura 3: Arquitectura propuesta", "Eq. 1: Esquema de encapsulación de claves"],
      "llaves_bibtex": ["Do2026_PQCAware", "Althobaiti2021_QuantumResistant"]
    },
    {
      "nro": 5,
      "titulo_seccion": "Metodología de Implementación y Evaluación",
      "objetivos": ["Describir implementación en hardware simulado/real", "Definir métricas de evaluación"],
      "subsecciones": ["5.1 Entorno Experimental", "5.2 Algoritmos Seleccionados (ML-KEM, ML-DSA)", "5.3 Métricas: Energía, Latencia y Overhead"],
      "insumos": ["Tabla 4: Parámetros de simulación"],
      "llaves_bibtex": ["Liu2024_PQC_IoT", "Do2026_PQCAware"]
    },
    {
      "nro": 6,
      "titulo_seccion": "Resultados y Análisis",
      "objetivos": ["Presentar datos de rendimiento", "Comparar con enfoques clásicos"],
      "subsecciones": ["6.1 Rendimiento Computacional", "6.2 Análisis de Seguridad", "6.3 Escalabilidad en Despliegues Masivos"],
      "insumos": ["Figura 4: Gráficos de consumo energético", "Tabla 5: Comparación benchmarks"],
      "llaves_bibtex": ["Do2026_PQCAware", "Liu2024_PQC_IoT"]
    },
    {
      "nro": 7,
      "titulo_seccion": "Discusión",
      "objetivos": ["Interpretar resultados", "Analizar limitaciones y trade-offs"],
      "subsecciones": ["7.1 Viabilidad Práctica", "7.2 Comparación con Estado del Arte", "7.3 Implicaciones para Estándares"],
      "insumos": [],
      "llaves_bibtex": ["Althobaiti2020_Cybersecurity", "Do2026_PQCAware"]
    },
    {
      "nro": 8,
      "titulo_seccion": "Conclusiones y Trabajos Futuros",
      "objetivos": ["Resumir hallazgos principales", "Proponer direcciones futuras"],
      "subsecciones": ["8.1 Conclusiones", "8.2 Limitaciones", "8.3 Trabajos Futuros"],
      "insumos": [],
      "llaves_bibtex": ["Liu2024_PQC_IoT", "Do2026_PQCAware"]
    }
  ]
}
```

```bibtex
@article{Liu2024_PQC_IoT,
  author    = {Liu, Tao and Ramachandran, Gowri and Jurdak, Raja},
  title     = {Post-Quantum Cryptography for Internet of Things: A Survey on Performance and Optimization},
  journal   = {arXiv preprint arXiv:2401.17538},
  year      = {2024},
  doi       = {10.48550/arXiv.2401.17538},
  url       = {https://arxiv.org/pdf/2401.17538},
  note      = {[Online]. Available: https://arxiv.org/abs/2401.17538}
}

@article{Althobaiti2021_QuantumResistant,
  author    = {Althobaiti, Osamah S. and Dohler, Mischa},
  title     = {Quantum-Resistant Cryptography for the Internet of Things Based on Location-Based Lattices},
  journal   = {IEEE Access},
  volume    = {9},
  pages     = {133975--133991},
  year      = {2021},
  doi       = {10.1109/ACCESS.2021.3114730},
  url       = {https://ieeexplore.ieee.org/document/9547310},
  note      = {[Online]. Available: https://ieeexplore.ieee.org/document/9547310}
}

@article{Althobaiti2020_Cybersecurity,
  author    = {Althobaiti, Osamah S. and Al-Rodhaan, Mznah and Al-Dhelaan, Abdullah},
  title     = {Cybersecurity Challenges Associated With the Internet of Things in a Post-Quantum World},
  journal   = {IEEE Access},
  volume    = {8},
  pages     = {157356--157381},
  year      = {2020},
  doi       = {10.1109/ACCESS.2020.3019346},
  url       = {https://ieeexplore.ieee.org/document/9176998},
  note      = {[Online]. Available: https://ieeexplore.ieee.org/document/9176998}
}

@article{Do2026_PQCAware,
  author    = {Do, Thi-Bac},
  title     = {A PQC-Aware Secure Communication Architecture for NB-IoT: Control-Plane Post-Quantum Onboarding with Lightweight Data-Plane Protection},
  journal   = {Engineering, Technology & Applied Science Research},
  year      = {2026},
  url       = {https://etasr.com/index.php/ETASR/article/view/17220},
  note      = {[Online]. Available: https://etasr.com/index.php/ETASR/article/view/17220}
}
```

```json
{
  "seccion_nro": 1,
  "titulo_seccion": "Introducción",
  "mapa_uso": {
    "Liu2024_PQC_IoT": {
      "razon_seleccion": "Proporciona encuesta exhaustiva sobre PQC en IoT con énfasis en rendimiento para dispositivos restringidos.",
      "guia_redaccion": "Usar en 1.1 y 1.2 para motivar el problema y destacar brechas en implementaciones actuales para NB-IoT.",
      "subseccion_destino": "1.1"
    },
    "Althobaiti2021_QuantumResistant": {
      "razon_seleccion": "Enfocado en criptografía resistente cuántica basada en lattices para IoT incluyendo NB-IoT.",
      "guia_redaccion": "Citar en 1.2 para introducir propuestas de autenticación y transmisión seguras en entornos NB-IoT.",
      "subseccion_destino": "1.2"
    }
  }
}
```

```json
{
  "seccion_nro": 2,
  "titulo_seccion": "Antecedentes y Estado del Arte",
  "mapa_uso": {
    "Liu2024_PQC_IoT": {
      "razon_seleccion": "Survey detallado de performance y optimizaciones PQC.",
      "guia_redaccion": "Usar en 2.3 para revisar algoritmos NIST y comparaciones en IoT.",
      "subseccion_destino": "2.3"
    },
    "Althobaiti2020_Cybersecurity": {
      "razon_seleccion": "Analiza desafíos de seguridad 3GPP IoT en contexto post-cuántico.",
      "guia_redaccion": "Integrar en 2.1 y 2.2 para discutir vulnerabilidades NB-IoT actuales.",
      "subseccion_destino": "2.1"
    },
    "Do2026_PQCAware": {
      "razon_seleccion": "Arquitectura específica PQC para NB-IoT.",
      "guia_redaccion": "Contrastar en 2.3 destacando enfoques híbridos control/data plane.",
      "subseccion_destino": "2.3"
    }
  }
}
```

```json
{
  "seccion_nro": 3,
  "titulo_seccion": "Amenazas Cibernéticas en Comunicaciones de Exploración Profunda",
  "mapa_uso": {
    "Althobaiti2021_QuantumResistant": {
      "razon_seleccion": "Propone solución lattice-based para amenazas en NB-IoT.",
      "guia_redaccion": "Usar para ejemplificar harvest-now-decrypt-later en escenarios remotos.",
      "subseccion_destino": "3.2"
    },
    "Liu2024_PQC_IoT": {
      "razon_seleccion": "Detalla impacto en dispositivos restringidos.",
      "guia_redaccion": "Citar métricas de overhead en 3.3.",
      "subseccion_destino": "3.3"
    }
  }
}
```

```json
{
  "seccion_nro": 4,
  "titulo_seccion": "Propuesta de Arquitectura de Seguridad Cuántica",
  "mapa_uso": {
    "Do2026_PQCAware": {
      "razon_seleccion": "Arquitectura PQC-aware directamente aplicable a NB-IoT.",
      "guia_redaccion": "Base principal para describir onboarding y protección en Fig. 3 y Eq. 1.",
      "subseccion_destino": "4.1"
    },
    "Althobaiti2021_QuantumResistant": {
      "razon_seleccion": "Complementa con enfoque location-based.",
      "guia_redaccion": "Integrar para robustez en entornos de exploración profunda.",
      "subseccion_destino": "4.2"
    }
  }
}
```

```json
{
  "seccion_nro": 5,
  "titulo_seccion": "Metodología de Implementación y Evaluación",
  "mapa_uso": {
    "Liu2024_PQC_IoT": {
      "razon_seleccion": "Proporciona benchmarks y optimizaciones relevantes.",
      "guia_redaccion": "Usar para justificar selección de algoritmos y métricas en 5.2-5.3.",
      "subseccion_destino": "5.2"
    },
    "Do2026_PQCAware": {
      "razon_seleccion": "Evaluación en plataforma NB-IoT real.",
      "guia_redaccion": "Adoptar metodología experimental similar.",
      "subseccion_destino": "5.1"
    }
  }
}
```

```json
{
  "seccion_nro": 6,
  "titulo_seccion": "Resultados y Análisis",
  "mapa_uso": {
    "Do2026_PQCAware": {
      "razon_seleccion": "Resultados empíricos en NB-IoT.",
      "guia_redaccion": "Base para tablas y figuras de rendimiento.",
      "subseccion_destino": "6.1"
    },
    "Liu2024_PQC_IoT": {
      "razon_seleccion": "Comparaciones amplias de PQC.",
      "guia_redaccion": "Usar para contextualizar resultados en 6.3.",
      "subseccion_destino": "6.3"
    }
  }
}
```

```json
{
  "seccion_nro": 7,
  "titulo_seccion": "Discusión",
  "mapa_uso": {
    "Althobaiti2020_Cybersecurity": {
      "razon_seleccion": "Perspectiva post-cuántica en 3GPP.",
      "guia_redaccion": "Contrastar limitaciones y estándares en 7.2-7.3.",
      "subseccion_destino": "7.2"
    },
    "Do2026_PQCAware": {
      "razon_seleccion": "Análisis de trade-offs prácticos.",
      "guia_redaccion": "Integrar para discusión de viabilidad.",
      "subseccion_destino": "7.1"
    }
  }
}
```

```json
{
  "seccion_nro": 8,
  "titulo_seccion": "Conclusiones y Trabajos Futuros",
  "mapa_uso": {
    "Liu2024_PQC_IoT": {
      "razon_seleccion": "Recomendaciones futuras en PQC-IoT.",
      "guia_redaccion": "Usar para proponer direcciones en 8.3.",
      "subseccion_destino": "8.3"
    },
    "Do2026_PQCAware": {
      "razon_seleccion": "Conclusiones específicas NB-IoT.",
      "guia_redaccion": "Sintetizar hallazgos principales.",
      "subseccion_destino": "8.1"
    }
  }
}
```