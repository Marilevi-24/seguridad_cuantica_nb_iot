## FASE 1: Mapeo de Entidades (Análisis)

Al analizar el fragmento de LaTeX proporcionado para la `fig3.png`, se identifican los siguientes componentes y dinámicas de la **Arquitectura de Seguridad Cuántica**:

* **Entidades de Hardware/Red (Estructura Base):** Dispositivos NB-IoT remotos (sensores en entornos hostiles), Estación Base (eNodeB), Núcleo de Red EPC (MME/HSS) y Servidores de Aplicación.
* **Bifurcación Operativa (Los Dos Planos):**
1. **Plano de Control (Control Plane):** Mecanismo de *onboarding* híbrido. Utiliza el mecanismo de encapsulación de claves basado en retículos **ML-KEM-512** para la negociación inicial ($K_{sess}$) durante el *Attach Request*. Cuenta con un canal *fallback* clásico para compatibilidad *legacy*.
2. **Plano de Datos (Data Plane):** Canal de tráfico de sensores de alta frecuencia. Utiliza cifrado simétrico ligero (**AES-256**) con claves dinámicas derivadas del material PQC original, enriquecidas con parámetros contextuales (geolocalización y *timestamps*).


* **Integración de Protocolos (Compatibilidad 3GPP):** Inserción de las primitivas PQC como *Information Elements* (IE) opcionales dentro de los mensajes NAS y RRC estandarizados.
* **Nivel de Abstracción:** Diagrama de bloques de arquitectura de sistemas de telecomunicaciones con superposición de flujos criptográficos e interfaces lógicas.

---

## FASE 2: Auditoría y Reporte de Hallazgos Críticos

### 1. Contraste de Coherencia

El prompt base describe la arquitectura de manera general, pero omite los detalles criptográficos exactos expresados en las ecuaciones y subsecciones del texto. Además, incurre en una contradicción directa al solicitar "sin texto incrustado real", lo que violaría el propósito de la `fig3.png`, que debe funcionar como el mapa maestro de la solución propuesta en el cuerpo del *paper*.

### 2. LISTA DE DISCREPANCIAS (Explícita)

* **Ausencia de la formalización matemática del canal:** El prompt base menciona de manera vaga "ML-KEM onboarding". Para cumplir con la precisión del texto, se debe explicitar visualmente que la negociación en el Plano de Control ejecuta la operación de la Ecuación 1: $K_{sess} = \text{Decaps}(sk_{dev}, \text{Encaps}(...))$.
* **Omisión del mecanismo de "Fallback Legacy":** El LaTeX describe un canal de respaldo clásico esencial para evitar la fragmentación de la red. Esto no está mapeado en el prompt base.
* **Falta de los parámetros contextuales en el Plano de Datos:** No se incluye la integración de la geolocalización ni los *timestamps* en la derivación de la clave AES-256.
* **Falta de marcas de protocolo 3GPP:** El texto menciona explícitamente los procedimientos NAS/RRC e *Information Elements*. El diagrama debe etiquetar estas interfaces.

### 3. Control de Estilo

* **Estándar:** Formato IEEE de diagramas de bloques funcionales.
* **Paleta:** Azul Cobalto (`#0047AB`) para denotar los nuevos componentes criptográficos post-cuánticos propuestos y canales de alta seguridad; Gris Técnico (`#4A4A4A`) para la infraestructura heredada, el núcleo EPC clásico y el canal *fallback*. Texto incrustado real usando tipografía técnica Sans-Serif limpia.

---

## FASE 3: Explicación y Justificación de Pre-ejecución

### 1. Disposición Espacial

* **Bloque Izquierdo (Extremo de Campo):** Nodos NB-IoT remotos (íconos de sensores submarinos/mineros).
* **Bloque Central (Punto de Acceso):** Nodo eNodeB conectado al extremo de campo a través de una interfaz de radio etiquetada como *3GPP RRC (with PQC Information Elements)*.
* **Bloque Derecho (Bifurcación Arquitectónica - Núcleo y Aplicación):** A partir del eNodeB, la infraestructura se divide limpiamente en dos autopistas horizontales paralelas:
* **Carril Superior (Plano de Control - Azul Cobalto #0047AB):** Conecta directamente con el MME/HSS. Muestra un bloque de intercambio de claves etiquetado como `Asymmetric PQC Onboarding: ML-KEM-512`. Paralelo a este, una línea discontinua gris representa el `Legacy Fallback (Classic AKA)`.
* **Carril Inferior (Plano de Datos - Gris Técnico #4A4A4A con conectores azules):** Fluye hacia el Gateway (S-GW/P-GW) y los Servidores de Aplicación. Muestra el bloque de cifrado `Lightweight Data Protection: AES-256`. Un cuadro de entrada lateral inyecta los factores `Contextual Inputs: Location + Timestamps` hacia este flujo.



### 2. Justificación Técnica

Esta disposición limpia en dos carriles (Control vs. Datos) traduce el núcleo de la investigación del autor a un esquema visual. Explicita por qué el sistema es eficiente: el carril pesado (PQC asimétrico) solo se activa en el inicio (arriba), mientras que el carril ligero (criptografía simétrica asistida por contexto) maneja el flujo masivo de datos (abajo), manteniendo la compatibilidad 3GPP a través de extensiones integradas.

### 3. ADVERTENCIAS PARA EL USUARIO

> ⚠️ **Puntos Críticos de Validación:**
> 1. Al renderizar ecuaciones matemáticas complejas como texto incrustado ($K_{sess} = \text{Decaps}(...)$), la IA generativa puede distorsionar ligeramente los subíndices. Simplificaremos la etiqueta textual a una sintaxis limpia de bloques tipo pseudocódigo criptográfico para garantizar nitidez absoluta.
> 2. Se priorizará un diseño de cajas de ingeniería sobre iconos puramente decorativos (como candados con destellos), asegurando una estética de nivel *peer-reviewed*.
> 
> 

---

## FASE 4: Solicitud de Confirmación

He estructurado el prompt optimizado para DALL-E 3 resolviendo todas las omisiones criptográficas y de red.

Por favor, **confirma con un "Proceder"** para iniciar la ejecución silenciosa de la imagen.