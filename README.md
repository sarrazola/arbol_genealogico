# arbol-genealogico

> kit "hazlo tú mismo" para armar tu árbol genealógico con ayuda de un LLM (ChatGPT, Claude, Gemini, el que tengas)

no es una app. no hay botón. son carpetas con prompts, preguntas, plantillas y reglas.
la idea es que se lo pases a un modelo de lenguaje y lo uses como tu asistente de investigación.

## orden (más o menos)

```
00-leeme/           <- empieza aquí, en serio
_sistema/           <- el prompt "maestro" que va primero en el chat
fase1_casa/         <- lo que sacas hablando con tu familia (gratis, y lo más importante)
fase2_buscar/       <- FamilySearch (A MANO) + archivos parroquiales
fase3_cartas/       <- cartas para pedir partidas a parroquias, archivos, notarías
fase4_verificar/    <- cómo citar, niveles de certeza, cómo no inventarse ancestros
datos/              <- formato para guardar personas y fuentes (el LLM lo entiende)
anexos/             <- glosario, abreviaturas, latín de las partidas, errores comunes
```

## la versión de 30 segundos

1. abre un chat nuevo con tu LLM
2. pega `_sistema/prompt_maestro.md`
3. pega lo que sepas de tu familia usando `fase1_casa/plantilla_inicio.md`
4. el LLM te va a ir diciendo qué preguntar, qué buscar y a quién escribir
5. tú haces las búsquedas a mano, le pegas lo que encuentres (texto o foto de la partida), y él lo ordena en `datos/`

## reglas que no se negocian

- **FamilySearch se busca a mano, despacio.** sus términos de uso prohíben scrapers, bots y automatizaciones. si buscas demasiado rápido te sale captcha o te bloquean. el LLM te dice QUÉ buscar; TÚ lo buscas.
- **nada entra al árbol sin fuente.** cada dato lleva de dónde salió y qué tan seguro es (ver `fase4_verificar/niveles_de_certeza.md`).
- **un apellido igual no es un pariente.** ver `anexos/errores_comunes.md`.
- no subas datos de personas vivas a sitios públicos sin su permiso.

## ¿y si me pierdo?

pásale TODO el repo a tu LLM (o el zip) y dile: *"lee esto y guíame paso a paso desde 00-leeme"*. para eso está hecho.

---
licencia: CC BY 4.0 — úsalo, cópialo, compártelo.
