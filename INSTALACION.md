# 🚀 Instalación de NexusIA

Guía para instalar NexusIA en una PC con Windows 10 u 11. Tardas entre **5 y 30 minutos**, según la opción y tu internet.

---

## Antes de empezar

| Necesitas | Detalle |
|---|---|
| Windows 10 u 11 | De 64 bits |
| Internet | Solo durante la instalación y para usar las IA en la nube |
| Espacio libre | 200 MB (Ligero) o 8 GB (Completo) |
| Navegador | Chrome, Edge o Firefox |

> 💡 **Si tienes VPN**, déjala encendida durante la instalación: algunas descargas (GitHub, Ollama) pueden fallar sin ella.

---

## Paso 1 · Descomprimir

1. Clic derecho sobre **NexusIA.zip** › **Extraer todo…** › **Extraer**.
2. Abre la carpeta **NexusIA** que se creó.

> ⚠️ No ejecutes el instalador desde dentro del ZIP sin descomprimir: no encontrará los archivos.

## Paso 2 · Ejecutar el instalador

1. Doble clic en **Instalar NexusIA.bat**.
2. Si Windows muestra **«Windows protegió su PC»**: pulsa **Más información** › **Ejecutar de todas formas**.
   *(Aparece porque el archivo no tiene firma comercial; es normal.)*

Se abre una ventana negra que muestra la memoria (RAM) y el espacio libre de tu PC, y te **recomienda** una opción.

## Paso 3 · Elegir la opción

| Opción | Qué instala | Tamaño | Elígela si… |
|---|---|---|---|
| **[1] LIGERO** ⭐ | NexusIA + **FreeLLMAPI** (une cientos de IA gratis en la nube) | ~110 MB | Tu PC es normal o tiene poca memoria. **Es la recomendada para casi todos.** |
| **[2] COMPLETO** | Lo de Ligero + **Ollama** + modelo **gemma3:4b** (IA que funciona en tu PC, sin internet) | ~4,5 GB | Tienes **8 GB de RAM o más**, 8 GB de disco libre y quieres IA aunque se caiga el internet. |
| **[3] SOLO NexusIA** | Solo la aplicación | 1 MB | Ya tienes FreeLLMAPI u Ollama instalados, o vas a usar solo claves de Gemini, Groq, etc. |

Escribe el número y pulsa **Enter**.

### ¿Cuál elijo? En dos preguntas

```
¿Tu PC tiene 8 GB de RAM o más?
 ├─ No  → [1] LIGERO
 └─ Sí  → ¿Se te va mucho el internet y quieres IA sin conexión?
           ├─ Sí → [2] COMPLETO
           └─ No → [1] LIGERO  (puedes añadir Ollama más tarde)
```

> ℹ️ La IA de Ollama en tu PC es **más lenta** y **menos lista** que las de la nube, pero funciona sin internet y sin límites. Con poca RAM puede ir muy lenta.

## Paso 4 · Esperar

El instalador hace solo:

1. Copia NexusIA a `C:\Users\TU_USUARIO\AppData\Local\NexusIA`.
2. Crea el acceso directo **NexusIA** en el **Escritorio** y en el **Menú Inicio**.
3. Descarga e instala **FreeLLMAPI** (opciones 1 y 2).
4. Descarga e instala **Ollama** y el modelo **gemma3:4b** (solo opción 2; puede tardar mucho).

Si una descarga falla, **reintenta sola** varias veces. Si aun así no puede, te abre la página de descarga para que lo bajes a mano (ver *Problemas* más abajo).

Al terminar, **NexusIA se abre sola en el navegador** con el **Asistente de configuración**.

## Paso 5 · Asistente de configuración (dentro de NexusIA)

Son 4 pantallas:

| Pantalla | Qué haces |
|---|---|
| **1. Estado** | Ves qué está conectado: FreeLLMAPI ✓, Ollama ✓/—. |
| **2. Clave de FreeLLMAPI** | Copia tu clave y pégala (ver abajo). Pulsa **Probar**. |
| **3. Proveedores gratis** | Consigue al menos 1 o 2 claves gratis y pégalas **en el panel de FreeLLMAPI** (enlaces abajo). |
| **4. Prueba final** | NexusIA envía una pregunta de prueba. Si sale ✓, ya está. |

### Cómo copiar la clave de FreeLLMAPI

- **Opción A:** junto al reloj de Windows, clic derecho en el icono de **FreeLLMAPI** › **Copy Key**.
- **Opción B:** abre el panel `http://127.0.0.1:31415` › **Keys** › **Copy API key**.

La clave empieza por `freellmapi-…`. Pégala en el asistente y pulsa **Probar**.

### Claves gratis para FreeLLMAPI (todas sin tarjeta)

Ábrelas, crea la clave, cópiala y pégala en el panel de FreeLLMAPI (sección de proveedores):

| Proveedor | Enlace | Nota |
|---|---|---|
| **Google Gemini** ⭐ | https://aistudio.google.com/apikey | La mejor para empezar. Lee imágenes. |
| **Groq** | https://console.groq.com/keys | Muy rápida. |
| **OpenRouter** | https://openrouter.ai/settings/keys | Muchos modelos «:free». |
| **Mistral** | https://console.mistral.ai/api-keys | Buena en español. |
| **Cerebras** | https://cloud.cerebras.ai | Muy rápida. |
| **NVIDIA** | https://build.nvidia.com | Modelos grandes. |
| **Cloudflare** | https://dash.cloudflare.com/profile/api-tokens | Necesita también el ID de cuenta. |

> 💡 Cuantas más claves pongas, más créditos diarios gratis tienes: cuando uno se agota, FreeLLMAPI pasa al siguiente solo.

---

## Uso diario

1. Doble clic en **NexusIA** (Escritorio o Menú Inicio).
2. Se abre una ventana pequeña minimizada (**no la cierres**) y NexusIA en el navegador.
3. FreeLLMAPI y Ollama se abren solos si estaban cerrados.

Para cerrar: cierra la pestaña y la ventana minimizada de NexusIA.

---

## IA de pago (opcional)

Si algún día quieres más calidad, en NexusIA ⚙ **Configuración › Motor IA** pon la clave de **OpenAI**, **Anthropic (Claude)**, **DeepSeek** o **xAI**. Solo se usan si tú las activas; el motor ⚡ Automático sigue prefiriendo las gratis.

---

## Problemas y soluciones

| Problema | Solución |
|---|---|
| «Windows protegió su PC» | **Más información › Ejecutar de todas formas**. |
| La ventana se cierra enseguida | Clic derecho en **Instalar-NexusIA.ps1** › **Ejecutar con PowerShell**. |
| No descarga FreeLLMAPI | Enciende la VPN y repite. O bájalo a mano: https://github.com/tashfeenahmed/freellmapi/releases/latest (archivo `FreeLLMAPI.Setup.….exe`), instálalo y vuelve a ejecutar el instalador con la opción **[3]**. |
| No descarga Ollama | Bájalo a mano: https://ollama.com/download/OllamaSetup.exe. Luego, en una ventana de comandos: `ollama pull gemma3:4b`. |
| Se cortó la corriente a mitad | Vuelve a ejecutar **Instalar NexusIA.bat**. Lo ya instalado no se repite. |
| «FreeLLMAPI no está abierto» | Ábrelo desde el Menú Inicio y recarga NexusIA (F5). |
| «Invalid API key» | La clave de FreeLLMAPI está mal copiada. Cópiala otra vez (Copy Key) y pégala en ⚙ Configuración. |
| Ninguna IA responde | Revisa que tengas al menos una clave de proveedor puesta en el panel de FreeLLMAPI. |
| Quiero repetir la configuración | ⚙ Configuración › **🧭 Asistente de configuración**. |

El registro de la instalación queda en `C:\Users\TU_USUARIO\AppData\Local\NexusIA\instalacion.log`. Envíalo al soporte si algo falla.

---

## Desinstalar

1. Borra la carpeta `C:\Users\TU_USUARIO\AppData\Local\NexusIA` y los accesos directos **NexusIA**.
2. FreeLLMAPI y Ollama se quitan desde **Configuración de Windows › Aplicaciones**.

> ⚠️ Tus agentes y conversaciones se guardan en el navegador. Antes de desinstalar, en NexusIA usa ⚙ **Configuración › Mis datos › 💾 Exportar todo** para tener copia.

---

<p align="center"><b>NexusIA</b> · by <b>HiSpaNet</b> · WhatsApp +53 5508 1288</p>
