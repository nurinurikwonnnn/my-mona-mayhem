<!-- l10n-sync: source-file="workshop/06-bonus.md" -->
# 🎉 Extras y ampliaciones

---

¡Has creado una aplicación de GitHub Battle totalmente funcional! Ahora puedes ir más allá con estos **retos abiertos**.

<!-- track:vscode:start -->
Usa **Agent Mode** para todos estos retos: describe lo que quieres y deja que Copilot te ayude a crearlo.
<!-- track:vscode:end -->

<!-- track:cli:start -->
Usa Copilot CLI para todos estos retos: combina el contexto de `@file`, `/plan`, el modo normal y `/review` según convenga.
<!-- track:cli:end -->

---

## 🏆 Reto 1: Anuncio del ganador

Cuando se hayan cargado los dos gráficos de contribuciones, compara los totales y muestra un anuncio dinámico del ganador.

**Qué crear:**
- Compara el total de contribuciones de ambos usuarios
- Si hay un ganador claro, muestra **"🏆 {username} WINS! 🏆"** con un estilo de celebración
- Si las contribuciones son iguales, muestra **"🤝 IT'S A TIE! 🤝"**
- Añade animaciones o confeti para darle más vistosidad

**Sugerencia de prompt:**
> After both users' contribution data loads, compare total contributions and display a winner banner. Show "🏆 {username} WINS! 🏆" if one user has more contributions, or "🤝 IT'S A TIE! 🤝" if equal. Make it visually exciting with CSS animations.

---

## 🏆 Reto 2: Contador de rachas

Calcula y muestra la racha más larga de contribuciones consecutivas de cada usuario.

**Qué crear:**
- Analiza los datos de contribuciones día a día
- Encuentra la secuencia más larga de días consecutivos con al menos una contribución
- Muestra de forma destacada el recuento de la racha de cada usuario
- Resalta quién tiene la racha más larga

**Sugerencia de prompt:**
> Add a streak counter feature that analyzes each user's contribution data to find their longest consecutive contribution streak. Display "🔥 Longest Streak: X days" for each user below their contribution graph.

---

## 🏆 Reto 3: Historial de batallas

Guarda los resultados de las batallas para que los usuarios puedan ver sus enfrentamientos anteriores.

**Qué crear:**
- Guarda cada resultado de batalla en `localStorage` (nombres de usuario, totales, ganador y marca de tiempo)
- Añade una sección **"Recent Battles"** debajo del área principal de batalla
- Muestra los resultados de las últimas 5–10 batallas
- Añade un botón «Clear History»

**Sugerencia de prompt:**
> Save battle results to localStorage after each comparison. Add a "Recent Battles" section that displays the last 10 battles with usernames, contribution totals, the winner, and when the battle happened. Include a "Clear History" button.

---

## 🏆 Reto 4: Efectos de sonido

Añade efectos de sonido de arcade retro con la Web Audio API; no necesitas archivos externos.

**Qué crear:**
- Sonido de **moneda al insertarla** al hacer clic en el botón «Battle!»
- Sonido de **potenciación** cuando los resultados se carguen correctamente
- Sonido de **explosión** cuando se produzca un error (usuario no encontrado o fallo de la API)
- Un botón para activar o silenciar el sonido

**Sugerencia de prompt:**
> Add retro arcade sound effects using the Web Audio API (no audio files). Play a coin insert sound on battle start, a power-up sound when results load, and an explosion sound on errors. Generate the sounds programmatically with oscillators and gain nodes. Include a mute toggle.

---

## 🏆 Reto 5: Secuencia de batalla animada

Crea expectación con una cuenta atrás dramática antes de mostrar los resultados.

**Qué crear:**
- Al hacer clic en «Battle!», muestra una superposición a pantalla completa
- Anima: **"3..."** → **"2..."** → **"1..."** → **"⚡ FIGHT! ⚡"**
- Después, muestra los gráficos de contribuciones con una entrada dramática
- Usa animaciones CSS o temporizadores de JavaScript

**Sugerencia de prompt:**
> Add an animated battle sequence when the user clicks "Battle!". Show a countdown overlay: "3..." then "2..." then "1..." then "⚡ FIGHT! ⚡" with each step lasting about 1 second. After the countdown, reveal the results with a slide-in animation.

---

## 🏆 Reto 6: Leyenda de contribuciones

Añade una leyenda de escala de colores que coincida con la paleta del gráfico de contribuciones.

**Qué crear:**
- Una leyenda horizontal con los niveles de intensidad de las contribuciones
- Etiquetas de **"Less"** a **"More"**
- Usa la paleta de colores real de la respuesta de la API de contribuciones de GitHub
- Colócala cerca de los gráficos de contribuciones

**Sugerencia de prompt:**
> Add a contribution legend below the graphs showing the color scale from the API's color palette. Display a row of colored squares ranging from "Less" (lightest) to "More" (darkest), matching the actual contribution level colors returned by the API.

---

## 🏆 Reto 7: Comparte los resultados

Permite que los usuarios compartan el resultado de su batalla con un solo clic.

**Qué crear:**
- Un botón **«📋 Share Results»** que aparezca después de una batalla
- Copia al portapapeles un resumen de texto con formato
- Incluye nombres de usuario, totales de contribuciones y quién ha ganado
- Muestra brevemente un mensaje de confirmación «Copied!»

**Sugerencia de prompt:**
> Add a "📋 Share Results" button that copies a formatted battle summary to the clipboard. The summary should include both usernames, their contribution totals, and who won. Use the Clipboard API and show a brief "Copied to clipboard!" confirmation.

---

<!-- track:cli:start -->
## 💻 Extras del CLI

Si quieres explorar más funciones de Copilot CLI después del taller principal:

- Usa `copilot -p "Write a conventional commit message for the current git diff"` para generar una respuesta puntual que puedas copiar en Git.
- Ejecuta `/share file` para guardar la sesión como Markdown y consultarla más adelante.
- Usa `/session` y `/session plan` para inspeccionar cómo está siguiendo el CLI el trabajo actual.
<!-- track:cli:end -->

## 🎊 ¡Enhorabuena!

¡Has completado el taller **Mona Mayhem: GitHub Battle**! Esto es lo que has conseguido:

### Lo que has creado

- ✅ Una **aplicación web completa con varias páginas** a partir de una especificación de diseño
- ✅ Una **página de inicio** con temática de arcade retro y diseño adaptable
- ✅ Una **arena de batalla** que obtiene y compara datos reales de contribuciones de GitHub
- ✅ **Gráficos de contribuciones interactivos** con niveles de actividad identificados por colores
- ✅ Mejoras de **gestión de errores, estados de carga y accesibilidad**
- ✅ **Diseño adaptable** para distintos dispositivos

### Lo que has practicado

| Habilidad | Qué has practicado |
|---|---|
| **Ingeniería del contexto** | Proporcionar a Copilot los archivos, instrucciones y restricciones adecuados |
| **Planificación** | Generar y perfeccionar planes de implementación antes de programar |
| **Programación agéntica** | Delegar en Copilot tareas de varios pasos y archivos |
| **Iteración del diseño** | Partir de una propuesta visual y perfeccionarla hasta obtener un resultado pulido |
| **Disciplina de revisión** | Inspeccionar los cambios generados por IA antes de confirmarlos con un commit |

### 🚀 Sigue aprendiendo

- 📺 [Canal de YouTube de VS Code](https://www.youtube.com/@code) — Consejos, tutoriales y novedades
- 📖 [Documentación de GitHub Copilot](https://docs.github.com/en/copilot) — Documentación oficial y guías
- 💻 [Documentación de GitHub Copilot CLI](https://docs.github.com/en/copilot/how-tos/copilot-cli) — Instalación, comandos slash y prácticas recomendadas
- 🌟 [Awesome GitHub Copilot](https://github.com/stefanprodan/awesome-github-copilot) — Recursos y ejemplos de la comunidad
- 🛠️ [Talleres de Copilot Dev Days](https://github.com/github/copilot-dev-days) — Más talleres prácticos como este

---

## 🙏 ¡Gracias!

¡Gracias por participar en este taller! Has visto cómo GitHub Copilot puede acelerar todas las fases del desarrollo: desde la planificación y el diseño hasta la implementación y el pulido. Las técnicas que has practicado aquí sirven para cualquier proyecto, framework y escala. ¡Ahora ve y crea algo increíble! 🚀
