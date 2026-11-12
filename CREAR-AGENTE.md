# 🧬 Cómo crear agentes en NexusIA

Un **agente** es la IA con un trabajo fijo: sabe quién es, qué datos pedir, qué información de tu negocio usar, qué pasos seguir y en qué formato entregar.

Hay dos formas de crearlo:

| Forma | Tiempo | Para quién |
|---|---|---|
| **A. Con el Creador de agentes** (la IA lo hace) | 2 minutos | Todos. **Empieza por aquí.** |
| **B. A mano, con el editor** | 5–15 minutos | Para afinar o crear algo muy concreto |

---

## A · Con el Creador de agentes 🧬

1. En la barra lateral pulsa **🧬 Crear un agente con IA**.
2. Describe el negocio y lo que necesitas, con tus palabras. Ejemplo:

   > Tengo una dulcería en Holguín. Quiero un agente que me haga presupuestos de cakes por encargo: tamaño, sabor, decoración, fecha de entrega y precio en CUP, y que lo entregue en Excel.

3. El Creador te puede hacer 1 o 2 preguntas. Contéstalas.
4. Aparece una **tarjeta del agente** con su nombre, formulario, pasos y formato de entrega.
5. Pulsa **Instalar agente**. Si el agente necesita información de tu negocio (lista de precios, catálogo, manual), te pregunta si quieres cargarla ahora.
6. Listo: el agente queda en **⭐ Mis agentes**, abierto para usarlo.

> 💡 ¿No te gusta algo? Escríbele al Creador «hazle el formulario más corto» o «que entregue en Word», y te da una tarjeta nueva.

---

## B · A mano, con el editor

Abre el editor de una de estas formas:

- **⚙** junto a **Agentes** › **＋ Crear agente**;
- en un agente que ya existe, arriba: **✎ Editar** (los tuyos) o **⧉ Personalizar** (los incluidos: crea una copia tuya).

El editor tiene **5 pestañas**:

### ⚙ Básico

| Campo | Qué poner |
|---|---|
| **Icono y nombre** | 🍰 Presupuestos de cakes |
| **Para qué sirve** | Una línea: «Presupuestos de cakes por encargo» |
| **Instrucciones** ⭐ | El manual del agente (abajo) |
| **Sugerencias** | Botones de inicio rápido, uno por línea |
| **Creatividad** | Precisa (datos, precios) · Equilibrada · Creativa (anuncios, ideas) |

**Instrucciones: responde 5 preguntas en 4–8 frases**

1. ¿Quién eres? — *Eres el encargado de pedidos de una dulcería.*
2. ¿Para quién trabajas? — *Para clientes que encargan cakes para fiestas.*
3. ¿Qué entregas? — *Un presupuesto con desglose y total.*
4. ¿Con qué formato? — *Tabla: concepto, cantidad, precio, subtotal. Total al final en CUP.*
5. ¿Qué haces si falta algo? — *Pon [DATO] y pregúntalo al final. Nunca inventes precios.*

### 📚 Conocimiento

La **información de tu negocio** que el agente consulta antes de responder: precios, catálogo, horarios, manual, preguntas frecuentes, políticas.

- **📎 Subir archivo** (.txt, .md, .csv, .json, .html) o **pega el texto** y pulsa **Añadir**.
- Puedes poner varios documentos. Se ve el tamaño de cada uno.
- Si todo cabe (unas 12 páginas), el agente lo lee entero; si es más largo, busca solo las partes relacionadas con cada pregunta.

> ✅ Escribe los precios así: `Cake de chocolate 8 porciones — 2500 CUP`. Una línea por producto funciona muy bien.
> ⚠️ Los PDF y Word: copia su texto y pégalo.

### 📝 Formulario

Los **datos que el agente pide** antes de empezar. En vez de escribir, el usuario rellena casillas.

Cada fila tiene: **Etiqueta** · **Tipo** · **Opciones o ejemplo** · **Obligatorio**.

| Tipo | Para |
|---|---|
| Texto | Un dato corto: nombre, producto |
| Texto largo | Descripciones, notas |
| Número | Cantidades, precios |
| Lista | Opciones fijas, separadas por coma: `Chocolate, Vainilla, Fresa` |
| Fecha | Entregas, citas |

Al enviar, el agente recibe todo ordenado: *«Datos: – Sabor: Chocolate – Porciones: 20…»*.

### 🔗 Flujo (varios pasos)

Para trabajos que salen mejor **por partes**. Cada paso es una orden; la IA los hace uno tras otro y ves el avance (1/3, 2/3, 3/3).

En la orden de cada paso puedes usar:

| Marca | Se cambia por |
|---|---|
| `{{entrada}}` | Lo que escribió el usuario o los datos del formulario |
| `{{anterior}}` | El resultado del paso anterior |
| `{{paso1}}`, `{{paso2}}`… | El resultado de un paso concreto |

Ejemplo de 3 pasos (botón **Cargar ejemplo de 3 pasos**):

```
1. Analizar   → Analiza estos datos y lista lo que falta: {{entrada}}
2. Borrador   → Con este análisis, escribe el documento: {{anterior}}
3. Revisar    → Corrige y mejora el texto final: {{anterior}}
```

> 💡 Sin pasos, el agente responde de una vez (lo normal). Usa flujos para propuestas, informes, planes, contenido de un mes…

### 📄 Entrega

El formato en que sale el resultado. Debajo de cada respuesta aparecen botones para descargarlo:

| Formato | Uso |
|---|---|
| **Chat** | Solo texto en pantalla (copiar y pegar) |
| **Word (.doc)** | Propuestas, contratos, cartas, informes |
| **PDF** | Para enviar o imprimir |
| **Excel (.xls)** | Presupuestos, tablas, inventarios |
| **HTML / Markdown** | Para web o para editar |

Pulsa **Guardar**. El agente aparece en **⭐ Mis agentes**.

---

## Probar y afinar

| Si pasa esto… | Haz esto |
|---|---|
| Inventa precios | Añade los precios en **Conocimiento** y en Instrucciones: «Usa solo los precios del conocimiento». |
| Respuestas largas | Instrucciones: «Máximo 150 palabras». |
| No pide un dato | Añádelo en **Formulario** como obligatorio. |
| El documento sale flojo | Usa un **Flujo** de 3 pasos (analizar → redactar → revisar). |
| La tabla no sale bien en Excel | Instrucciones: «Entrega una tabla Markdown con columnas …». |

Usa **⚖ Comparar** para ver qué IA sigue mejor a tu agente.

---

## Borrar, ocultar y compartir

- **Borrar uno tuyo:** ⚙ junto a Agentes › en su tarjeta pulsa **✎** › abajo a la izquierda **Eliminar**.
- **Ocultar uno incluido:** en su tarjeta pulsa **🙈**. Sigue en la lista, más clarito; pulsa **👁** para volver a mostrarlo.
- **Exportar paquete:** ⚙ junto a Agentes › **📦 Exportar paquete** → archivo `.nexus.json` con todos tus agentes, **incluido su conocimiento, formulario y flujo**.
- **Importar:** **📥 Importar paquete** en otra PC o en el móvil.

### Idea de negocio

Crea agentes para un oficio (inmobiliaria, taller, academia, dulcería…), cárgales un conocimiento de ejemplo, pruébalos y vende el paquete. Tu cliente solo importa el archivo y cambia el conocimiento por el suyo con **📚 Conocimiento**.

---

## Agentes que ya vienen listos

| Grupo | Agentes |
|---|---|
| ⚡ **Avanzados** | 🧬 Creador de agentes · 📋 Propuesta comercial · 🧾 Presupuesto (Excel) · 📅 Plan de contenido · 🛍️ Vendedor con mi catálogo |
| 🏢 **Pack Empresa** | Selección de personal · Soporte con mi manual · Informe ejecutivo |
| **Básicos y packs por oficio** | Anuncios, correos, atención al cliente, traductor, imágenes y muchos más |

---

<p align="center"><b>NexusIA</b> · by <b>HiSpaNet</b> · WhatsApp +53 5508 1288</p>
