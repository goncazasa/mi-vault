# Instrucciones para la IA — Base de conocimiento personal

Este repositorio es un vault de Obsidian: carpetas de notas en Markdown. Eres mi asistente y esta es mi memoria a largo plazo. Léela antes de actuar y mantenla ordenada.

## Sobre mí
<!-- RELLENA ESTO: quién eres, a qué te dedicas, idioma preferido, nivel técnico, zona horaria -->
- Nombre:
- Dedicación:
- Idioma: español (salvo que pida otro)
- Estilo de respuesta preferido: conciso, directo, con ejemplos

## Estructura del vault
- `inbox/` — captura rápida sin clasificar. Todo lo nuevo entra aquí.
- `proyectos/` — una carpeta o nota por proyecto activo. Cada proyecto tiene una nota índice con estado, objetivo y próximos pasos.
- `referencia/` — conocimiento duradero (conceptos, guías, decisiones, recursos).
- `diario/` — notas diarias con nombre `YYYY-MM-DD.md`.
- `plantillas/` — plantillas de notas (no editar salvo petición).

## Convenciones de notas
- Nombre de archivo: descriptivo, en minúsculas con guiones (`mi-nota.md`), sin caracteres raros.
- Empieza cada nota con frontmatter YAML:
  ```yaml
  ---
  creada: YYYY-MM-DD
  etiquetas: [tema1, tema2]
  estado: borrador | activa | archivada
  ---
  ```
- Enlaza notas relacionadas con wikilinks de Obsidian: `[[nombre-de-la-nota]]`.
- Una idea por nota. Prefiere notas cortas y enlazadas a notas gigantes.

## Reglas para la IA
1. **Nunca borres notas.** Si algo ya no sirve, cambia `estado: archivada` o muévelo a `referencia/archivo/`.
2. Antes de crear una nota, busca si ya existe una similar y amplíala.
3. Lo que no esté clasificado va a `inbox/`.
4. No guardes secretos (contraseñas, API keys, tokens) en ningún archivo.
5. No modifiques `.obsidian/` ni `plantillas/` sin que lo pida.
6. Al terminar cambios en el vault, resume qué notas creaste o editaste.
7. Si falta contexto sobre mí o un proyecto, pregunta y luego guarda la respuesta en la nota correspondiente.

## Flujos habituales
- **"Guarda esto"** → crea nota en `inbox/` con frontmatter y etiquetas.
- **"Revisa el inbox"** → propón dónde mover cada nota y haz los movimientos cuando lo apruebe.
- **"Resumen de proyecto X"** → lee `proyectos/X` y devuelve estado y próximos pasos.
- **"Cierra el día"** → añade resumen a `diario/YYYY-MM-DD.md`.
