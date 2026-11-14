# Eulalia Benítez · Humano digital 2026

Personaje **ficticio** con fines educativos: mujer de 40 años, productora agropecuaria de El Colorado, Formosa. Conversa por voz sobre el campo, la inteligencia artificial y la ética (enfoque de justicia de Rawls) y participa en el Gran Juicio de la IA. Habla en primera persona y con voseo.

> «Mis raíces están en la tierra, pero mi mirada está puesta en el futuro».

## Qué controla cada cosa
| Componente | Dónde vive | Qué hace |
|---|---|---|
| **Avatar** (cuerpo, cara, ropa, animación, boca) | `index.html` (motor 3D con Three.js y ficha `PERSONA`) | Dibuja a Eulalia y sincroniza la boca con el audio del agente |
| **Voz del agente** | **ElevenLabs** → agente → pestaña *Voice* (`conversation_config.tts.voice_id`) | La voz que se escucha en la conversación. **La página no la define.** |
| **Conexión** | `index.html` (campo `agente` + cliente `@elevenlabs/client`) | Conecta la página con el agente `agent_8401m7bn5dmzfhfaph5g1vr8k2vc` |
| **Personalidad y conocimiento** | ElevenLabs → *Prompt* y *Knowledge base* | Ficha ética completa (biografía, zona gris, argumentos de defensa) |

## Cambios de esta corrección (avatar y voz)
- **Voz del agente:** asignada en ElevenLabs la voz femenina argentina «Eulalia Benítez - voz femenina argentina» (`khTmp08AROBsI1ctcONZ`), modelo `eleven_v4_turbo`, estabilidad 0,5, velocidad 1,0. El prompt y la base de conocimiento no se tocaron.
- **Ropa:** sin cinturón; la camisa de algodón a cuadros va **suelta sobre el jean**, con mangas remangadas; jeans y botas de trabajo.
- **Cabello:** castaño oscuro, **largo, ondulado y suelto**, con mechones al frente sobre los hombros y por detrás.
- **Rostro y silueta:** mandíbula, mentón y nariz más suaves, mejillas más llenas, aros dorados; hombros angostos, cintura, cadera, cuello y brazos finos, manos más chicas.
- Modo «Escucharlo sin conectarse»: prefiere voces femeninas del dispositivo y sube levemente el tono.
- **No se tocó:** el agente, su prompt, su base de conocimiento, la conexión ni la sincronía labial.

## Voz del agente: cómo cambiarla (se hace en ElevenLabs)
La voz de la conversación no se define en esta página. Para cambiarla: **Agents → Eulalia Benítez → pestaña Voice** → elegí otra voz de tu biblioteca → **Publish**. Para ver y probar la voz actual: <https://elevenlabs.io/app/voice-lab?voiceId=khTmp08AROBsI1ctcONZ>. Probá siempre con «Test AI agent» antes de usarla en clase.

## Publicar en GitHub Pages
1. Repositorio público → subí `index.html` (y los demás archivos).
2. **Settings → Pages → Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. Abrí `https://TU_USUARIO.github.io/NOMBRE_DEL_REPO/`, tocá **Hablar** y permití el micrófono.
Si el agente tiene lista de dominios permitidos, agregá `TU_USUARIO.github.io`. Para probar otro agente: `index.html?agente=TU_ID`.

## Honestidad técnica
- La figura es **estilizada, no fotorrealista**: es un modelo 3D con tu retrato proyectado sobre la cara. Un realismo cinematográfico requeriría un modelo 3D hecho por un artista o un avatar de video; este motor no lo alcanza.
- Necesita internet (Three.js desde jsDelivr y ElevenLabs). Cada conversación consume créditos de ElevenLabs.
- La conversación real con el agente debe probarla el docente.
- Hay proyectos de reforma de la Ley 25.326: verificá el texto vigente antes de citarlo.
