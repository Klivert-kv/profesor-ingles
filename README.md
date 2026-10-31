# Profesor de inglés con memoria

¿Le has pedido a una IA que te enseñe inglés y a la semana ya no
recordaba nada? Este profesor guarda tu nivel, tus errores y tu
vocabulario en una libreta, y planifica cada clase a partir de ahí.
Funciona en Claude, ChatGPT y Gemini.

* Clases a tu ritmo, del tiempo que tengas cada día
* No depende del chat: abre una conversación nueva y sigue donde lo dejaste
* Mide tu nivel con una prueba corta y arranca desde ahí
* Eres su único alumno: toda su atención es para ti
* Anota tus errores y el vocabulario que fallas, y te los repasa hasta que los domines
* Si vas bien, sube la dificultad; si te cuesta, va más despacio

## Resultados

Lo probé yo mismo como alumno durante 9 días (del 22 al 31 de octubre de 2026):

* **8 de 9 días de clase**: solo falté uno, y al volver retomó donde lo dejé
* **Diagnóstico inicial**: me ubicó en un nivel A2 rumbo a B1
* **Ruta propia**: me preguntó mis metas con el inglés y armó las clases a partir de ellas

## Cómo funciona la memoria

Todo lo que el profesor sabe de ti vive en un documento llamado
**"Inglés – Perfil y progreso"** (la libreta): tu nivel, tu objetivo, la ruta
de temas, tus errores frecuentes y el vocabulario que toca repasar.

| Plataforma | Dónde vive la libreta |
|---|---|
| Claude | El profesor la crea y la actualiza solo, como documento o archivo |
| ChatGPT y Gemini | Al final de cada clase te la entrega; la guardas y la pegas (o subes) al empezar la siguiente |

## Cómo usarlo

### En la app de Claude
1. Descarga `profesor-ingles.zip` de este repositorio
2. En Configuración, activa la ejecución de código y archivos
3. En la sección de Skills, pulsa "Añadir skill" y sube el .zip
4. Abre un chat y escribe: "Comencemos la clase de inglés de hoy"

### En Claude Code
1. Copia la carpeta `claude/profesor-ingles` en `~/.claude/skills/`
2. Abre Claude Code y escribe: "Comencemos la clase de inglés de hoy"

### En ChatGPT (GPT personalizado)
1. Entra en ChatGPT y ve a "Explorar GPT" → "Crear"
2. Abre la pestaña "Configurar" y ponle de nombre "Profesor de inglés"
3. Copia todo el texto de [`chatgpt/instrucciones.md`](chatgpt/instrucciones.md) y pégalo en "Instrucciones"
4. Pulsa "Crear" y escribe: "Comencemos la clase de inglés de hoy"

### En Gemini (Gem)
1. Entra en Gemini y ve a "Explorar Gems" → "Nuevo Gem"
2. Ponle de nombre "Profesor de inglés"
3. Copia todo el texto de [`gemini/instrucciones.md`](gemini/instrucciones.md) y pégalo en "Instrucciones"
4. Guarda el Gem, ábrelo y escribe: "Comencemos la clase de inglés de hoy"

> En ChatGPT y Gemini, guarda la libreta que te da al final de cada clase.
> Al día siguiente, pégala en tu primer mensaje.

## Qué le puedes decir

- "Comencemos la clase de inglés de hoy" → lee tu libreta y da la clase que toca
- "¿Cómo se dice *me quedé dormido* en inglés?" → te responde corto, con un ejemplo
- "Corrígeme esto: *I have 20 years*" → te corrige y anota el error si se repite
- "¿Cómo voy?" → te resume tu progreso con datos de la libreta
- "Repasemos vocabulario" → te pregunta las palabras que toca repasar hoy

## Privacidad

Las instrucciones son solo texto: no ejecutan código ni se conectan a ningún
servicio. La libreta guarda únicamente datos para aprender y se queda contigo,
en tu cuenta o en tu dispositivo. No escribas en ella contraseñas ni datos
personales sensibles.

## Estructura

```
profesor-ingles/
├── README.md
├── LICENSE
├── profesor-ingles.zip        ← la skill de Claude, lista para subir
├── claude/
│   └── profesor-ingles/
│       └── SKILL.md
├── chatgpt/
│   └── instrucciones.md
└── gemini/
    └── instrucciones.md
```

## Licencia

[MIT](LICENSE): puedes usarlo, copiarlo y modificarlo, citando al autor.
