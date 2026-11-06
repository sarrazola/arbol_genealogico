# formato de datos

el LLM guarda el árbol así (JSON). puedes pedirle "ESTADO" y pegarlo en `datos/mi_arbol/personas.json`.

```json
{
  "id": "P001",
  "nombre": "Nombre Apellido1 Apellido2",
  "sexo": "M|F",
  "nacimiento": {"fecha": "1891-03-12", "aprox": false, "lugar": "...", "fuente": "F003", "certeza": "DOCUMENTADO"},
  "bautismo": {"fecha": "...", "lugar": "...", "fuente": "F003"},
  "matrimonios": [{"conyuge": "P002", "fecha": "...", "lugar": "...", "fuente": "F010", "certeza": "..."}],
  "defuncion": {"fecha": null, "lugar": null, "fuente": null},
  "padre": {"id": "P010", "certeza": "PROBABLE", "fuente": ["F003","F004"]},
  "madre": {"id": "P011", "certeza": "DOCUMENTADO", "fuente": ["F003"]},
  "padrinos": ["texto libre"],
  "notas": "contradicciones, dudas, pendientes",
  "pendiente": ["buscar matrimonio de los padres en <parroquia> 1880-1890"]
}
```

fuentes aparte:
```json
{"id": "F003", "cita": "Bautismo de ..., libro 7, f. 45v ...", "visto_en": "FamilySearch ark:/...", "archivo_local": "1891_bautismo_Gomez_Juana.jpg"}
```

ejemplo completo (gente inventada) en `ejemplo/`.

¿quieres verlo como árbol gráfico? pídele al LLM: *"convierte personas.json a GEDCOM"* e impórtalo en cualquier programa de genealogía, o pídele un diagrama Mermaid.
