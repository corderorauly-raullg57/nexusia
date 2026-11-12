# 📘 Guía de uso de NexusIA

NexusIA reúne **cientos de IA gratis** en una sola pantalla y las convierte en **agentes** que trabajan para tu negocio: redactan, presupuestan, atienden clientes, hacen documentos e imágenes.

> ¿Aún no la instalaste? Mira **INSTALACION.md**.

---

## 1 · La pantalla

```
┌──────────────┬──────────────────────────────────────────┐
│ 🧬 Crear un  │  Agente elegido  [Cambiar ▾] [✎ Editar]  │
│  agente con IA│  ┌────────────────────────────────────┐ │
│              │  │ Formulario o sugerencias            │ │
│ ⚡ Avanzados  │  └────────────────────────────────────┘ │
│ Básicos      │                                          │
│ Packs        │  Respuestas  ·  📄 Word PDF Excel …      │
│ ⭐ Mis agentes│                                          │
│ Conversaciones│ [📎] [⚖] [ escribe aquí…      ] [➤]     │
│ ⚙ Configurar │   Motor: ⚡ Automático ▾                 │
└──────────────┴──────────────────────────────────────────┘
```

- **Izquierda:** agentes y conversaciones guardadas.
- **Centro:** el agente activo. Si tiene formulario, rellénalo y pulsa **Enviar**; si no, toca una sugerencia o escribe.
- **Abajo:** 📎 adjuntar (imágenes, textos), ⚖ comparar dos IA, el cuadro de texto y el **motor**.

## 2 · El motor ⚡ Automático

No tienes que elegir IA. El motor prueba en orden **FreeLLMAPI → Gemini → Groq → OpenRouter → … → Ollama** y usa la primera que responde. Si una se queda sin créditos del día, pasa a la siguiente sola.

Si quieres una concreta, ábrela en **Motor ▾** y elígela.

## 3 · Los agentes

| Tipo | Qué hacen |
|---|---|
| ⚡ **Avanzados** | Piden datos con **formulario**, trabajan en **varios pasos**, usan **tu información** y entregan **documentos** |
| **Básicos** | Un papel fijo: anuncios, correos, atención al cliente, traductor… |
| **Packs** | Grupos por oficio y el **🏢 Pack Empresa** |
| ⭐ **Mis agentes** | Los que creas o instalas tú |

### Cómo usar un agente avanzado (ejemplo: 📋 Propuesta comercial)

1. Elígelo en la barra lateral.
2. Rellena el formulario: cliente, servicio, precio… (los campos con * son obligatorios).
3. Pulsa **Enviar**. Verás el avance: *Analizar 1/3 → Redactar 2/3 → Revisar 3/3*.
4. Debajo del resultado: **Word · PDF · Excel · HTML · MD**. Pulsa el que necesites y se descarga.

### Agentes con tu información (📚)

Algunos agentes, como **🛍️ Vendedor con mi catálogo** o **Soporte con mi manual**, necesitan tus datos. Verás un aviso: pulsa **Cargar mis documentos**, pega tu lista de precios o tu manual y guarda. A partir de ahí responde **solo con tus datos**.

### Crear tus agentes

Pulsa **🧬 Crear un agente con IA** y descríbele tu negocio. Todos los detalles en **CREAR-AGENTE.md**.

## 4 · Imágenes

Elige el agente **🎨 Creador de imágenes** y describe lo que quieres en español. Para cambiarla: «hazla más oscura», «ponle fondo blanco».

## 5 · Configuración ⚙

| Sección | Para |
|---|---|
| **Motor IA** | Claves de FreeLLMAPI, Ollama, Gemini, Groq… y las de pago (opcionales) |
| **Mis datos** | Tu nombre e **instrucción general** (lo que todos los agentes saben de ti: ciudad, negocio, forma de pago) |
| **🧭 Asistente de configuración** | Repetir la configuración guiada |
| **Mis datos › 💾 Exportar todo** | Copia de agentes, conversaciones y ajustes |

> 💡 Escribe en **Instrucción general** algo como: *«Vivo en Holguín, Cuba. Tengo una dulcería. Mis clientes pagan por Transfermóvil. Precios en CUP.»*

## 6 · Consejos

- **Haz copia** cada semana: ⚙ › Mis datos › 💾 Exportar todo. Si se va la corriente no se pierde nada, pero la copia te protege si cambias de PC.
- **Las IA gratis pequeñas a veces fallan**: pulsa ↻ (Otra respuesta) o prueba otra en el motor.
- **No cierres la ventanita minimizada** de NexusIA mientras la usas: es la que conecta con FreeLLMAPI y Ollama.
- **Sin internet**: solo funciona Ollama (si instalaste la opción Completa).

---

<p align="center"><b>NexusIA</b> · by <b>HiSpaNet</b> · WhatsApp +53 5508 1288</p>
