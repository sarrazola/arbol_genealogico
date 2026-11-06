# cómo usar esto (de verdad)

## opción A: chat largo (la fácil)
1. chat nuevo.
2. pega `_sistema/prompt_maestro.md` completo.
3. pega `fase1_casa/plantilla_inicio.md` llena con lo que sepas (aunque sea poquito).
4. sigue lo que te diga. cada vez que encuentres algo, pégalo.
5. cada ~20 mensajes pídele: *"dame el estado actual en el formato de datos/formato_personas.md"* y guárdalo en un archivo. si el chat se pone lento o se olvida cosas, abres uno nuevo, pegas el prompt maestro + ese archivo y sigues.

## opción B: proyecto / carpeta (la buena)
si tu LLM permite "proyectos" o subir archivos (Claude Projects, ChatGPT Projects, NotebookLM, etc.):
- sube todo este repo como conocimiento del proyecto
- pon `_sistema/prompt_maestro.md` como instrucciones
- ve subiendo tus fotos de partidas y tu `personas.json` a medida que crece

## opción C: agente con acceso a archivos
si usas un agente que lee/escribe archivos (Claude Code, Cursor, etc.), clona el repo y dile:
*"lee 00-leeme y _sistema; vamos a trabajar en datos/mi_arbol/. no navegues FamilySearch por mí, solo dime qué buscar."*

## qué NO esperar
- el LLM no tiene acceso mágico a registros. si te "cita" una partida que no le diste, es inventada. ver `fase4_verificar/anti_alucinacion.md`.
- vas a llegar a muros. normal. para eso están las cartas (`fase3_cartas/`).
