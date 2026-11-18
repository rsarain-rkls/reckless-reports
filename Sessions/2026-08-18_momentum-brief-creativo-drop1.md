# Sesión: Momentum Brief Creativo Drop 1
**Fecha:** 2026-08-18 11:33
**Proyecto:** Momentum / Reckless Reports

---

**Usuario**
/analyze con dos transcripts de llamadas de Google Meet (Aug 10 y Aug 12) de Momentum. Quería ver el objetivo o la idea principal de cada llamada para profundizar el concepto y generar una idea clara de qué quiero hacer.

**Claude**
Analizó ambas llamadas. El Aug 10 fue la sesión creativa de 2 horas donde se definió el concepto del video de lanzamiento Drop 1 (ángel/diablo, counter, buzo como protagonista, dron). El Aug 12 confirmó la collab con Misael Nove (60K seguidores, chef/creator) y el lanzamiento del Drop 1 para el jueves.

Creó reportes HTML en reckless-reports:
- `reports/momentum-drop1-sesion-aug10/index.html` — sesión completa con video concept + colección verano
- Intentó crear `reports/momentum-misael-collab-drop1/` pero fue interrumpido

---

**Usuario**
te tire otra llamada lpm — mandó el transcript del Aug 10 (2 horas, Rodrigo + Mati + Sacca + Santy)

**Claude**
Analizó la llamada del 10 de agosto. Dos bloques principales:
1. Brainstorm creativo del video de lanzamiento Drop 1
2. Revisión de colección Drop 2 / Verano

Creó `reports/momentum-drop1-sesion-aug10/index.html` con:
- 5 temas core (buzo como psicomagia, Messi vs Cristiano, el contador, el pionero, 3 outfits verano)
- JTBD
- Simple Stick
- PR/FAQ
- Sprint plan semana 11-26 Ago
- Concepto video estructura completa
- Notion structure

Deployó a reckless-reports en Vercel (cuenta makeouthills-projects, que resultó ser la cuenta de Rodrigo, no la del usuario).

---

**Usuario**
porque te demoras tanto, no quiero que me armes nada en vercell, borra eso de la skill. quiero que analices con toda esa data y me des información valiosa para poder empezar a hacer el trabajo. no me des más directrices, entra de una, explica por qué, anda por partes.

**Claude**
Directo, sin reportes:

Lo primero que llama la atención: el concepto del video ya está resuelto desde el 10 de agosto, pero nadie lo tiene escrito en un lugar claro.

La sesión del 10 fue 2 horas donde cada uno tiró una capa — Sacca con ángel/diablo, Mati con el counter y el buzo como protagonista, Rodrigo unificando con el pionero y la comunidad. El resultado es sólido pero se quedó en el aire.

La idea central: el video no es sobre Momentum como marca — es sobre un momento universal. El buzo es el objeto que marca el antes y el después. No requiere que nadie te conozca para conectar.

Lo segundo: hay una tensión no resuelta entre dos finales — el apocalíptico de Mati (vos el único sobreviviente) vs el modelo Messi de Rodrigo (pionero que activa a otros). Terminaron acordando el segundo pero el arco narrativo no quedó definido desde ese final hacia atrás. Eso hay que resolver antes de grabar.

Pregunta: ¿esto reemplaza el video del jueves o es otra cosa?

---

**Usuario**
tengo una idea, te la leo — dictó por audio un concepto completo de cortometraje: "La Pandemia de la Procrastinación". Dos personajes (Carmen/Mati = Bruce Wayne rico y vacío; Nero/Rodrigo = clase media que sube por mérito). Un abuelo narrador estilo Atahualpa Yupanqui. Juan como presentador de noticias. Counter basado en población argentina. El buzo como artefacto mágico que combate la "enfermedad". Estructura de película con dos narrativas paralelas al estilo Sopranos.

**Claude**
Respondió con dos observaciones clave:

1. La metáfora de pandemia es el mejor insight — activa memoria muscular. Cuando alguien escucha "hay una nueva pandemia", su cuerpo ya sabe lo que es. El hack es redirigir ese miedo hacia la procrastinación.

2. El abuelo-narrador estilo Atahualpa Yupanqui es lo que hace que todo lo demás funcione. Sin eso, es otra historia de acción personal. Con esa voz, tiene melancolía, tiempo, peso de algo que ya pasó antes.

Pregunta: ¿esto reemplaza el video del jueves o es otra cosa?

---

**Usuario**
Esto es el video entero que sale el jueves. No lo limitemos. Lo podemos hacer. Estos tres días vamos a estar muy locos pero tiene dirección e idea clara. Armamelo en ese coso (el HTML). Se lo puedo presentar a los chicos.

**Claude**
Creó `reports/momentum-brief-creativo-drop1/index.html` con:

**Secciones:**
- 01 La Idea Madre: "La procrastinación es la pandemia del hombre moderno. Y el buzo es el artefacto que encontramos para combatirla." + por qué funciona la metáfora + el contador (46M habitantes Argentina)
- 02 Los Personajes:
  - CARMEN (Mati): Bruce Wayne argentino, 22-24, campo, vacío a pesar de tenerlo todo, forja el artefacto, primer en documentar en redes
  - NERO (Rodrigo): 21, familia trabajadora, ciudad, encuentra el video de Carmen, multiplica el mensaje
  - EL ABUELO (voz de Rodri): narrador estilo Atahualpa Yupanqui, La Pampa, observa desde tercera persona como Dios a sus nietos
  - JUAN (Sacca): presentador de noticias, voz institucional del miedo, aparece 3 veces
- 03 El Arco Narrativo completo: 6 actos (Apertura → La Pandemia → El Descenso → El Forjador → El Encuentro → El Contagio Bueno → Cierre)
- 04 Dirección Creativa: tono película (no reel), música tanguera, paleta apagada→luz, truco producción (misma toma x3 distinto vestuario)
- 05 Lo Que Graba Cada Uno: brief por persona (Mati, Rodri, Juan)
- 06 La Narración del Abuelo: tono, instrucción de grabación, fragmentos VO por acto

---

**Usuario**
me encanto, fijate de solucionar lo de vercell

**Claude**
Detectó el problema: el CLI de Vercel estaba autenticado con la cuenta de Rodrigo (makeouthills-projects), no con la cuenta del usuario (Amore / amoresconsideratto@gmail.com). Los deploys quedaban en "Building..." sin completar y mostraban "You Need Access" al intentar verlos.

Solución: pidió al usuario hacer `vercel logout` y `vercel login` con el email de Amore. Una vez reconectado, borró el directorio `.vercel` y redesplegó.

Resultado: **`reckless-reports-beta.vercel.app`** — cuenta de Amore, funciona, público.

Links finales:
- Brief Creativo Drop 1: `reckless-reports-beta.vercel.app/reports/momentum-brief-creativo-drop1`
- Lanzamiento Drop 1 (reporte anterior): `reckless-reports-beta.vercel.app/reports/momentum-drop1-launch`

---

**Usuario**
quiero cambiarle algo al personaje de Nero — "capaz me proyecto mucho y bardea al cheto, formatealo para que se entienda como la diferencia entre el otro"

**Claude**
Modificó la descripción de Nero en el HTML. Cambios:
- Eliminó "No es el típico cheto. Sube por lo que construye."
- Reemplazó por: "Su punto de partida es distinto al de Carmen, no mejor ni peor: simplemente otro camino hacia la misma lucha."
- En energía: cambió "El que viene de abajo y sube con otros" por "El puente entre los dos mundos — el que recibe el mensaje y lo multiplica hacia su gente."

Commit + push + deploy. URL actualizada en `reckless-reports-beta.vercel.app`.

---

**Archivos creados/modificados en esta sesión:**

| Archivo | Acción |
|---|---|
| `reports/momentum-drop1-sesion-aug10/index.html` | Creado |
| `reports/momentum-misael-collab-drop1/` | Directorio creado, no completado |
| `reports/momentum-brief-creativo-drop1/index.html` | Creado y editado |
| `vercel.json` | Modificado — agregado `framework: null, buildCommand: "", outputDirectory: "."` |
| `.vercel/` | Eliminado y recreado con cuenta Amore |

**Deploy final:** `reckless-reports-beta.vercel.app` (cuenta amoresconsideratto@gmail.com)

---
*Log guardado: 2026-08-18 11:33*
