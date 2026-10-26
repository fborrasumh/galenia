# GalenIA

Galénica II: estabilidad, sistemas dispersos, industria y envasado. Aplicación web de un solo fichero.

**Usar la app:** https://fborrasumh.github.io/galenia/

**Idiomas:** español (por defecto), inglés, portugués; selector en la barra superior (o `?lang=en` / `?lang=pt` en la URL).

## Qué hace

- **Temario:** las cuatro unidades didácticas de la guía docente de Galénica II (1680) —estabilidad de medicamentos, sistemas dispersos heterogéneos, industria farmacéutica y envasado—, con sus temas de teoría y práctica, los doce resultados de aprendizaje (que el estudiante marca cuando los domina) y las ideas clave de cada unidad.
- **Laboratorio de cálculo:** cinética de degradación de orden 0, 1 y 2 (t₉₀ y t½ con gráfica), Arrhenius por regresión de ln k frente a 1/T con extrapolación a la temperatura de conservación, HLB requerido de la fase oleosa y proporción de dos emulgentes, ley de Stokes con análisis de sensibilidad, clasificación reológica (newtoniano, plástico, pseudoplástico, dilatante) con detección de tixotropía por el área de histéresis, y tablas de ICH Q1A(R2), zonas climáticas y grados del Anexo 1 de las GMP de la UE.
- **Problemas con solución calculada:** nueve tipos (t₉₀ desde k o desde t½, orden cero, energía de activación, caducidad a 25 °C desde 40 °C, Q₁₀, mezcla de emulgentes, HLB requerido y Stokes) con variantes reproducibles por semilla. Si la respuesta no coincide (margen del 2 %), el código recalcula el problema con los errores típicos (°C en lugar de K, diámetro por radio, logaritmo decimal, t½ por t₉₀, fracciones cambiadas…) y explica cuál se ha cometido. Solución paso a paso.
- **Simulacro:** 32 preguntas de 5 alternativas sobre las cuatro unidades, como el examen de la guía, con explicación inmediata, opción de dejar en blanco, resumen por unidad sin nota y repaso de las falladas. Incluye el cálculo del valor esperado de arriesgar con la penalización de −1/3.
- **Casos con IA:** siete casos profesionales (diseño de un estudio de estabilidad, solución magistral inestable, emulsión O/W, suspensión que se apelmaza, zona de llenado aséptico, desviación en el agua purificada con plan PHVA y elección de envase). El tutor de IA devuelve comentarios y preguntas por cada elemento esperado; el código comprueba que cada cita que atribuye al estudiante aparece literalmente en su respuesta, ignora identificadores inventados, retira las frases que ponen nota o copian la respuesta orientativa y avisa de cifras que no están en el material. Autocomprobación y respuesta orientativa sin IA.
- **Progreso:** resumen, qué repasar, calculadora de la nota con los criterios de evaluación continua y no continua de la guía, informe en Word (sin librerías externas) y copia en JSON.

## Cómo se usa la IA

Solo en «Casos con IA», con la propia clave de OpenAI, Google Gemini o Anthropic Claude. La clave se guarda solo en el navegador. No hace falta servidor. Todo lo demás (cálculos, problemas, simulacro, nota, informes) funciona sin clave y sin conexión con ningún proveedor. El botón «Ver un ejemplo» muestra el tutor con un resultado precalculado, sin usar la IA.

## Privacidad

El progreso, las respuestas y la clave se guardan solo en el navegador (IndexedDB y localStorage). Al pedir comentarios al tutor sale hacia el proveedor elegido el enunciado del caso y la respuesta del estudiante, con correos, DNI/NIE y teléfonos enmascarados; antes del primer envío de la sesión se muestra lo que sale y se pide confirmación. El JSON exportado no contiene la clave. No se deben escribir datos de pacientes reales.

## Límites

Es material de estudio: no sustituye a las clases, a la bibliografía de la guía ni al criterio del profesorado, y la calculadora de nota es orientativa. Las tablas normativas (ICH, Anexo 1) y los valores de HLB son orientativos y deben contrastarse con la versión vigente. Los comentarios del tutor los genera una IA y pueden ser incompletos o erróneos; el código verifica las citas, no la corrección técnica de los comentarios. Las preguntas, casos e ideas clave los ha redactado el equipo autor a partir de la guía y conviene que el profesorado de la asignatura los revise. Probado con IA simulada en los tres proveedores; no se ha probado con claves reales.

## Autoría

Fernando Borrás Rocher (Universidad Miguel Hernández de Elche) y Enrique Barrajón Catalán (Universidad Miguel Hernández de Elche).

Construida a partir de la guía docente de Galénica II (asignatura 1680, 4.º curso del Grado en Farmacia, UMH, curso 2026-2027), de la que Enrique Barrajón Catalán es profesor.

ORCID: Fernando Borrás Rocher [0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573) · Enrique Barrajón Catalán [0000-0001-8113-0795](https://orcid.org/0000-0001-8113-0795)

## Cómo citar

Borrás Rocher, F. y Barrajón Catalán, E. (2026). *GalenIA* (v1.0.0) [Software]. (DOI en trámite)

## Licencia

MIT. Véase [LICENSE](LICENSE).
