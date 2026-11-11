# 📘 Guía de NEXO IA

Todo lo que necesitas saber para sacarle el máximo partido a NEXO IA, de lo más básico a lo más avanzado.

> **En 30 segundos:** abre `nexo-ia.html`, elige un asistente a la izquierda, escribe y pulsa **Enter**. Ya funciona. Lo demás de esta guía sirve para que funcione **mejor**.

---

## Índice

1. [Abrir NEXO](#1-abrir-nexo)
2. [La pantalla](#2-la-pantalla)
3. [El motor de IA y el modo Automático](#3-el-motor-de-ia-y-el-modo-automático)
4. [Conseguir claves gratis](#4-conseguir-claves-gratis)
5. [Tu propia IA: FreeLLMAPI, Ollama, LM Studio](#5-tu-propia-ia-freellmapi-ollama-lm-studio)
6. [IA de pago (opcional)](#6-ia-de-pago-opcional)
7. [Asistentes](#7-asistentes)
8. [Packs por oficio](#8-packs-por-oficio)
9. [Crear tus asistentes y venderlos como paquete](#9-crear-tus-asistentes-y-venderlos-como-paquete)
10. [Comparar dos IA](#10-comparar-dos-ia)
11. [Crear imágenes](#11-crear-imágenes)
12. [Fotos y documentos](#12-fotos-y-documentos)
13. [Herramientas de cada respuesta](#13-herramientas-de-cada-respuesta)
14. [Conversaciones, búsqueda y exportar](#14-conversaciones-búsqueda-y-exportar)
15. [Tus datos y copias de seguridad](#15-tus-datos-y-copias-de-seguridad)
16. [Atajos de teclado](#16-atajos-de-teclado)
17. [Problemas frecuentes](#17-problemas-frecuentes)
18. [Privacidad](#18-privacidad)

---

## 1. Abrir NEXO

Hay dos formas:

| Forma | Cuándo usarla |
|---|---|
| **Doble clic en `nexo-ia.html`** | Siempre funciona. Usa las IA de Internet. |
| **Doble clic en `Abrir NEXO IA.bat`** | Si tienes FreeLLMAPI, Ollama o LM Studio en tu PC. Los abre y los conecta solos. |

Si usas el `.bat`, aparece una **ventana negra**. Puedes minimizarla, pero **no la cierres** mientras uses NEXO: es la que conecta tu IA local.

> 💡 Si Windows muestra «Windows protegió su PC», pulsa **Más información › Ejecutar de todas formas**. Pasa con cualquier archivo descargado.

---

## 2. La pantalla

```
┌──────────────┬────────────────────────────────────────────┐
│ NEXO IA      │  Título de la conversación   ⚡Automático ⬇ 🖨│
│ ＋ Nueva     ├────────────────────────────────────────────┤
│              │                                            │
│ ASISTENTES ⚙ │          (aquí aparecen los mensajes)       │
│ 💬 Chat      │                                            │
│ 📣 Anuncios  │                                            │
│ 🎨 Imágenes  │                                            │
│ …            ├────────────────────────────────────────────┤
│ CONVERSACION │ 📎 ⚖  Escribe tu mensaje…     ✨ 🎙 [Enviar]│
│ 🔎 Buscar    │                                            │
│ ● 3 IA   ◐ ⚙ │                                            │
└──────────────┴────────────────────────────────────────────┘
```

- **Izquierda:** asistentes, tus conversaciones y la configuración (⚙ abajo).
- **Arriba a la derecha:** qué IA usar (**⚡ Automático** por defecto), descargar ⬇ e imprimir 🖨.
- **Abajo:** adjuntar 📎, comparar ⚖, mejorar mensaje ✨, dictar 🎙 y enviar.
- **Abajo a la izquierda:** «● 3 IA disponibles» te dice cuántas IA tiene NEXO listas para usar. ◐ cambia entre modo claro y oscuro.

En el móvil, la barra izquierda se abre con **☰**.

---

## 3. El motor de IA y el modo Automático

Esta es la parte más importante de NEXO.

NEXO no depende de una sola IA. Tiene una **lista de IA** y en modo **⚡ Automático** hace esto con cada pregunta:

```
Tu pregunta ──► IA nº 1 ──¿responde?── sí ──► ✅ respuesta
                   │
                   no (caída, cuota agotada, bloqueada)
                   ▼
                IA nº 2 ──¿responde?── sí ──► ✅ respuesta
                   │
                   no
                   ▼
                  …hasta la última (AI Horde, siempre disponible)
```

Tú no notas nada: solo ves la respuesta. Debajo de cada respuesta aparece **qué IA contestó y con qué modelo**.

### Cambiar el orden

⚙ **Configuración › Orden automático**. Sube ↑ o baja ↓ cada IA. Las que están en gris no se usan: les falta la clave o son de pago (ver [sección 6](#6-ia-de-pago-opcional)).

### Usar una IA concreta

En el selector de arriba a la derecha, cambia **⚡ Automático** por la IA que quieras. Así solo se usa esa, sin saltos.

### Probar que todo funciona

⚙ **Configuración › Motor IA › 🔌 Probar conexiones**. Cada IA muestra:

| Estado | Significado |
|---|---|
| ✓ funciona (N modelos) | Lista para usar |
| ✕ clave incorrecta | Revisa que copiaste la clave completa |
| ✕ bloqueada para tu país | Ese servicio no funciona desde tu país; prueba con VPN o usa otra |
| ✕ cuota agotada | Se acabó lo gratis por hoy; NEXO usará otra |
| ✕ clave incorrecta o sin permiso (Pollinations) | Pollinations ya pide clave: créala gratis en enter.pollinations.ai y pégala en su casilla |
| sin configurar | Falta la clave |

---

## 4. Conseguir claves gratis

NEXO funciona sin claves gracias a **AI Horde**, una red gratis de voluntarios. Pero es lenta (de 20 segundos a 2 minutos) y no ve fotos. Con **una o dos claves gratis** NEXO se vuelve rápida y potente.

| IA | Dónde sacar la clave | Lo mejor que tiene |
|---|---|---|
| **Google Gemini** | aistudio.google.com/apikey | Muy buena en español y ve fotos |
| **Groq** | console.groq.com/keys | Rapidísima |
| **OpenRouter** | openrouter.ai/settings/keys | Decenas de modelos gratis en una cuenta |
| **Mistral** | console.mistral.ai/api-keys | Buena en español y en código |
| **Cerebras** | cloud.cerebras.ai | Modelos grandes y muy rápidos |
| **Pollinations** | enter.pollinations.ai | GPT-5 mini gratis y crear imágenes sin espera (la clave empieza por `pk_` o `sk_`) |

**Pasos para cada una:**

1. Entra en la web, crea una cuenta gratis y busca **API Keys › Create key**.
2. Copia la clave.
3. En NEXO: ⚙ **Configuración › Motor IA**, pégala en la casilla **Clave** de esa IA.
4. Pulsa **🔌 Probar conexiones**.

> 💡 **Recomendación:** empieza por **Gemini** y **Groq**. Con esas dos tienes de sobra para el día a día.
>
> 🔒 Ninguna de estas pide tarjeta para el nivel gratis. Si alguna te la pide, no la pongas y usa otra.

### El campo «Modelo»

Déjalo **vacío**: NEXO elige solo el mejor modelo disponible. Si quieres uno concreto, pulsa **⟳** para cargar la lista y elige.

---

## 5. Tu propia IA: FreeLLMAPI, Ollama, LM Studio

**«Mi IA propia»** conecta una IA que corre en tu computadora. Es gratis, no tiene cuotas y, con Ollama, funciona **sin Internet**. Es la **nº 1** del modo Automático.

### Con FreeLLMAPI (recomendado si ya lo tienes)

FreeLLMAPI junta muchas IA gratis (y Ollama) detrás de una sola dirección. NEXO la usa como si fuera una sola IA, y FreeLLMAPI elige el modelo por dentro.

1. Abre NEXO con **`Abrir NEXO IA.bat`**. FreeLLMAPI se abre solo.
2. ⚙ **Configuración › Motor IA › Mi IA propia**:
   - **Dirección:** aparece sola (`http://localhost:31490/v1`). Si está vacía, escríbela.
   - **Clave:** pega tu clave de FreeLLMAPI (empieza por `freellmapi-`). La sacas en FreeLLMAPI › **Keys › Copy API key**.
   - **Modelo:** vacío (usa `auto`).
   - **Modelo para fotos:** `gemma3:4b` (o cualquier modelo que vea imágenes).
3. **🔌 Probar conexiones** → ✓ funciona.

> Si ya tienes tus claves de Groq, Gemini, etc. dentro de FreeLLMAPI, **no hace falta** ponerlas también en NEXO. Ponerlas sirve solo de reserva por si FreeLLMAPI está cerrado.

### Con Ollama

1. Instala Ollama (ollama.com/download) y descarga un modelo, por ejemplo con `ollama pull gemma3:4b`.
2. Abre NEXO con **`Abrir NEXO IA.bat`**: detecta Ollama solo.
3. En **Mi IA propia**, deja la **clave vacía**. En **Modelo** escribe el que descargaste (`gemma3:4b`).

### Con LM Studio

Igual que Ollama: abre LM Studio, activa su servidor local y abre NEXO con el `.bat`.

---

## 6. IA de pago (opcional)

Para quien quiere la máxima calidad. Pagas por uso **directamente al proveedor**; NEXO no cobra nada.

| IA | Para qué destaca |
|---|---|
| **OpenAI** (ChatGPT) | Todoterreno, imágenes de alta calidad |
| **Anthropic Claude** | Redactar y programar |
| **DeepSeek** | Muy buena y de las más baratas |
| **xAI Grok** | Alternativa potente |
| **Personalizada 1 y 2** | Cualquier servicio compatible con OpenAI: Together, DeepInfra, Fireworks, Azure… |

### 💳 El interruptor de seguridad

En ⚙ **Configuración › Motor IA › IA de pago** está:

> ☐ **Usar las IA de pago en modo Automático**

- **Apagado (por defecto):** las IA de pago **nunca** se usan solas. Solo funcionan si las eliges tú arriba en el selector o en Comparar. Así nunca gastas sin darte cuenta.
- **Encendido:** entran en la cadena automática según el orden que pongas.

Las IA de pago aparecen marcadas con **💳** en todos los selectores.

### IA personalizada

Rellena: **Nombre**, **Dirección** (por ejemplo `https://api.together.xyz/v1`), **Clave** y **Modelo**. Si es gratis, desmarca «Es de pago».

---

## 7. Asistentes

Un asistente es una IA con **instrucciones especiales** para una tarea. Elige uno a la izquierda y cada conversación nueva usará sus instrucciones.

| Asistente | Para qué |
|---|---|
| 💬 Chat libre | Lo que quieras |
| 📣 Anuncios para WhatsApp | 3 versiones de anuncio (corta, media, con historia) |
| 🎨 Creador de imágenes | Dibuja lo que describes |
| 📱 Redes sociales | Posts, hashtags, guiones de reels, calendarios |
| 🤝 Atención al cliente | Respuestas listas para copiar |
| 👨‍💻 Programador | Código completo y explicaciones sencillas |
| 🌎 Traductor | Traducciones naturales |
| ✍️ Redactor y corrector | Corrige y mejora textos |
| 📧 Emails y cartas | Asunto + correo listo |
| 🎬 Guiones de video | Tabla escena por escena |
| 💡 Ideas de negocio | Estrategia, precios y ventas |
| 🖼️ Analista de imágenes | Describe, lee y revisa fotos |
| 📄 Resumidor | Ideas clave de textos y documentos |

Cada asistente muestra **sugerencias para empezar**: haz clic en una y listo.

---

## 8. Packs por oficio

Asistentes especializados para cada tipo de negocio. Se instalan con un clic:

⚙ junto a **Asistentes › 📦 Packs por oficio › Instalar**.

| Pack | Asistentes |
|---|---|
| 🍕 Restaurantes y comida | Carta y menú · Promo del día · Pedidos y reclamos |
| 💈 Belleza y barbería | Citas y recordatorios · Contenido de estilos · Clientes fieles |
| 👗 Tiendas y ropa | Fichas de producto · Catálogo WhatsApp · Cierre de ventas |
| 🔧 Servicios técnicos | Presupuestos · Diagnóstico explicado · Seguimiento y reseñas |
| 🎓 Profesores y cursos | Planificador de clases · Creador de exámenes · Explicador paciente |
| 💻 Freelancers | Propuestas · Cobros amables · Marca personal |

Para quitarlo: mismo lugar, **Quitar pack**.

---

## 9. Crear tus asistentes y venderlos como paquete

### Crear

⚙ junto a **Asistentes › ＋ Crear asistente** y rellena:

- **Icono y nombre.**
- **Para qué sirve:** una línea.
- **Instrucciones:** lo más importante. Di quién es, qué hace, qué debe preguntar y cómo responder. Ejemplo:

  > *Eres experto en ventas de autos usados en Latinoamérica. Cuando te den marca, modelo, año y precio, escribe un anuncio con gancho, 5 ventajas, estado del vehículo y llamada a la acción. Si falta el kilometraje, pregúntalo.*

- **Sugerencias:** una por línea (aparecen como botones al empezar).
- **Creatividad:** *Precisa* para datos y código, *Creativa* para anuncios e ideas.

Para modificar uno de los incluidos, usa **⧉ Duplicar** y edita tu copia.

### 📦 Paquetes: compartir o vender

- **Exportar paquete:** guarda todos tus asistentes en un archivo `.nexo.json`.
- **Importar paquete:** suma los asistentes de un archivo a los tuyos.

> 💰 **Idea de negocio:** crea packs para un nicho («20 asistentes para inmobiliarias», «Pack para nutricionistas») y véndelos. Tus clientes solo tienen que importarlos.

---

## 10. Comparar dos IA

La misma pregunta a **dos IA a la vez**, lado a lado.

1. Pulsa **⚖** (junto al clip).
2. Elige las dos IA en la barra que aparece.
3. Escribe y envía.
4. Lee las dos respuestas y pulsa **Seguir con esta** en la que prefieras: la conversación continúa con ella.

Para salir, pulsa **✕** en la barra de comparar.

> Sirve para elegir qué IA poner primero en tu orden automático, o para quedarte con la mejor idea de dos.

---

## 11. Crear imágenes

1. Elige el asistente **🎨 Creador de imágenes**.
2. Elige el **formato**: Cuadrado 1:1 · Vertical 9:16 (Estados y Reels) · Horizontal 16:9 · Post 4:5.
3. Describe la imagen **en español**: «Logo minimalista para una cafetería llamada Aroma, colores marrón y crema».
4. NEXO escribe una descripción profesional en inglés y la dibuja.
5. **⬇ Descargar imagen.** Con **↻** pides otra versión.

**Para cambiarla**, escribe lo que quieres cambiar: «hazla más oscura», «quita el texto», «ahora en estilo acuarela». NEXO recuerda la imagen anterior.

### Quién dibuja

| Servicio | Precio | Velocidad |
|---|---|---|
| AI Horde | Gratis, sin clave | 1-3 min (red comunitaria, con cola) |
| Pollinations | Gratis con su clave | Sin espera |
| OpenAI · Gemini | De pago | Casi instantáneo, máxima calidad |

Las de pago solo se usan con su clave y el **interruptor de pago encendido**.

---

## 12. Fotos y documentos

Puedes adjuntar con **📎**, **arrastrando** los archivos a la ventana o **pegando** (Ctrl+V) una captura.

- **Fotos:** la IA las ve. Pregunta «¿qué error muestra esta captura?», «extrae el texto», «mejora esta foto de producto». Necesitas una IA que vea fotos: Gemini, Groq, OpenRouter, Mistral o tu IA propia con `gemma3:4b`.
- **Documentos de texto:** `.txt`, `.csv`, `.md`, `.html`, `.json`, código… La IA los lee completos.
- **PDF o Word:** copia el texto y pégalo en el mensaje.

---

## 13. Herramientas de cada respuesta

Debajo de cada respuesta:

| Botón | Hace |
|---|---|
| ⧉ | Copiar la respuesta |
| 🔊 | Leerla en voz alta (con las voces de Windows, sin Internet) |
| ↻ | Pedir otra respuesta |
| ⏩ | Continuar si se cortó |

En los **bloques de código**: **Copiar** y **Descargar** (con la extensión correcta: `.html`, `.py`…).

En **tus mensajes**: **✎** para editarlo y reenviarlo. Borra lo que vino después y te deja corregir la pregunta.

En el compositor:

- **✨ Mejorar mi mensaje:** escribe tu idea a medias y pulsa ✨. NEXO la reescribe más clara y completa para que la IA responda mejor.
- **🎙 Dictar:** habla y se escribe solo (necesita Internet; Chrome o Edge).

---

## 14. Conversaciones, búsqueda y exportar

- Se **guardan solas** y siguen ahí si se va la corriente.
- **🔎 Buscar** busca en títulos y dentro de los mensajes.
- Pasa el ratón sobre una conversación: **✎** para renombrar, **🗑** para borrar.
- Arriba a la derecha: **⬇** descarga la conversación en Markdown y **🖨** la imprime o guarda como **PDF** (elige «Guardar como PDF» en la impresora).

---

## 15. Tus datos y copias de seguridad

⚙ **Configuración › Mis datos**:

- **Tu nombre:** para que la IA te trate por tu nombre.
- **Instrucción general:** contexto que se añade a **todas** las conversaciones. Ejemplo: *«Vivo en Cuba, vendo herramientas digitales, uso un tono cercano.»*
- **💾 Exportar todo:** un archivo con conversaciones, asistentes y ajustes. Marca «incluir mis claves» solo si es para ti.
- **📂 Importar copia:** para pasar todo a otra PC.

> ⚠️ Los datos viven en el navegador. Si borras los datos del navegador o cambias de navegador, haz antes una copia con **Exportar todo**.

---

## 16. Atajos de teclado

| Atajo | Acción |
|---|---|
| `Enter` | Enviar |
| `Shift` + `Enter` | Nueva línea |
| `Ctrl` + `K` | Buscar conversaciones |
| `Esc` | Detener la respuesta |
| `Ctrl` + `V` | Pegar una captura como adjunto |

---

## 17. Problemas frecuentes

| Ves | Solución |
|---|---|
| «Ninguna IA respondió» | Revisa tu conexión. Añade una clave gratis más. Pulsa **Probar conexiones** para ver cuál falla. |
| Mi IA propia: «no responde» | Abre NEXO con el `.bat` y no cierres la ventana negra. Comprueba que FreeLLMAPI u Ollama estén abiertos. |
| Mi IA propia: «clave incorrecta» | Copia otra vez la clave de FreeLLMAPI (**Copy API key**) y pégala completa. |
| «bloqueada para tu país» | Ese servicio no funciona desde tu país. Usa VPN o pon otra IA delante en el orden. |
| «cuota agotada» | Se acabó lo gratis de esa IA por hoy. NEXO usa otra; añade más claves para tener más reserva. |
| La IA no ve mi foto | Usa una IA que vea imágenes (Gemini, Groq, OpenRouter, Mistral) o pon `gemma3:4b` en «Modelo para fotos». |
| Las imágenes tardan mucho | Sin claves usa AI Horde (1-3 min). Con la clave gratis de Pollinations o una de pago son rápidas. |
| El dictado no funciona | Necesita Internet y Chrome o Edge. |
| Perdí mis conversaciones | Se borraron los datos del navegador. Importa tu última copia (**Mis datos › Importar copia**). |

---

## 18. Privacidad

- NEXO **no tiene servidor**: habla directamente desde tu computadora con cada IA.
- Tus **claves y conversaciones** se guardan **solo en tu navegador**.
- Cada IA recibe solo los mensajes de la conversación en la que la usas.

---

<p align="center"><b>NEXO IA</b> · by <b>HiSpaNet</b><br>
¿Dudas? WhatsApp <a href="https://wa.me/5355081288">+53 5508 1288</a> · hispa.net.world@gmail.com</p>
