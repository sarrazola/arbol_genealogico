# búsqueda indexada (Buscar → Registros)

1. pon nombre y PRIMER apellido solamente. los índices a veces no tienen el segundo.
2. lugar: el municipio o el departamento/provincia. si no sale nada, quita el lugar.
3. rango de años: ±5 al principio, luego ±10.
4. usa los filtros de **padre** y **madre**: buscar "Juan" con padre "José" y madre "María" funciona mejor que nombre + apellido.
5. prueba variantes (pídeselas al LLM con el prompt de `_sistema/prompts_extra.md`).
6. busca a los HERMANOS: si encuentras 6 bautizos con los mismos padres, ya tienes a la pareja, y el matrimonio está cerca.
7. cuando encuentres un registro: copia el texto del índice + el enlace (ark:/...) + **mira la imagen original**. el índice se equivoca.

pégale al LLM:
```
Encontré esto en FamilySearch (índice): <pega>
Imagen: <describe o adjunta foto/captura>
Enlace: <url>
Extrae datos, compáralos con el índice y dime qué buscar después.
```
