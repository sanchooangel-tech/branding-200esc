# DESIGN.md · Los 200 € escondidos

Sistema de marca de **Los 200 € escondidos**: ebook y cuenta de ahorro doméstico para hogares en España.
Fuentes: web en producción (200escondidos.pages.dev), ebook PDF, landing, reels, foto de perfil y biografías.
Instagram (@los200escondidos) no se pudo leer automáticamente: revisa el apartado 9.

---

## 1. Esencia de marca

| | |
|---|---|
| **Qué es** | Un reto de 30 días para encontrar dinero en los gastos de casa sin renunciar a nada |
| **Para quién** | Personas que trabajan y cobran en España, pero no saben dónde acaba su dinero a fin de mes |
| **Promesa** | Un método claro: 15 minutos al día, una tarea concreta, guiones listos para usar |
| **Lo que NO prometemos** | Cifras garantizadas. Los 200 € son un **potencial**, nunca una garantía |
| **Personalidad** | Práctica, honesta, tranquila, cercana. Un amigo que sabe de números, no un gurú |
| **Formato de cuenta** | Faceless: voz en off, manos, objetos, pantallas. No sale nadie a cámara |

**Concepto visual central:** *dinero escondido que aparece*. El «200» que se hunde en la ranura de una hucha es el símbolo de la marca.

---

## 2. Paletas de color

La marca tiene **dos mundos** que comparten un acento verde:
- **Oscuro (fintech):** web, reels, foto de perfil y cierres de vídeo.
- **Crema (editorial):** ebook, portada y material descargable.

### 2.1 Paleta oscura · Web, redes y vídeo

| Rol | Nombre | HEX | Uso |
|---|---|---|---|
| Fondo | Negro tinta | `#08090C` | Fondo principal, `theme-color` de la web |
| Superficie | Grafito | `#14161B` | Tarjetas, cajas |
| Superficie 2 | Grafito claro | `#1A1D23` | Tarjetas elevadas, hover |
| Texto | Blanco hueso | `#F5F5F2` | Titulares y cuerpo |
| Texto secundario | — | `rgba(245,245,242,.62)` | Párrafos de apoyo |
| Texto terciario | — | `rgba(245,245,242,.42)` | Notas, letra pequeña |
| Líneas | — | `rgba(245,245,242,.09)` / `.16` | Bordes, separadores |
| **Acento** | Verde salvia claro | `#A3D9A5` | Palabras destacadas, subtítulos activos, iconos |
| **CTA** | Verde ahorro | `#70C98A` | Botones de compra |
| Texto sobre CTA | Verde noche | `#06140B` | Texto dentro de botones verdes |
| Hover CTA | — | `#7DD497` | Estado hover |
| Verde profundo | — | `#3E8E5C` | Gráficos, degradados |
| Glow | — | `#1A2420` | Halo verde oscuro detrás de elementos clave |

### 2.2 Paleta crema · Ebook y material descargable

| Rol | Nombre | HEX | Uso |
|---|---|---|---|
| Fondo | Crema | `#F7F0E3` | Páginas del ebook, portada |
| Papel | Papel | `#FBF7EF` | Cajas claras |
| Crema 2 / 3 | — | `#EFE3CF` / `#E6D5BA` | Tablas, bloques alternos |
| Título | Cacao | `#3F2E24` | Titulares |
| Texto | Marrón texto | `#4A3A2F` | Cuerpo |
| Texto suave | — | `#8A7462` | Pies de foto, notas |
| **Acento** | Caramelo | `#A9733F` | La palabra *escondidos*, cifras destacadas |
| Etiqueta | Terracota | `#C46A3D` | Pill «RETO DE 30 DÍAS» |
| Secundario | Oliva | `#55614A` | Etiquetas, bordes, ranura en versión crema |
| Salvia | — | `#7E9172` | Detalles, iconos |
| Caja de tarea | Salvia pálida | `#E4E7D6` | Recuadros «Haz esto hoy» |
| Destacado cálido | Mostaza | `#D4A13F` | Monedas, sellos («30 días») |

### 2.3 Reglas de color
- El verde (`#70C98A` / `#A3D9A5`) solo se usa para **acción o dinero recuperado**. Nunca es decorativo.
- Nada de rojo para «gasto»: la marca no asusta, acompaña.
- **Prohibido el rosa.** Se quitó de la portada por no encajar.
- En fondos oscuros, como máximo un acento por pantalla.

---

## 3. Tipografías

| Rol | Fuente | Pesos | Dónde |
|---|---|---|---|
| Sans (cuerpo e interfaz) | **Inter** | 400 · 500 · 600 · 700 | Web, ebook, botones, textos largos |
| Serif display (web) | **Instrument Serif** | Regular + *Italic* | Titulares de la web |
| Serif editorial (ebook y marca) | **Lora** | 500–700 + *Italic* | Título del ebook, cabeceras, foto de perfil |
| Subtítulos de vídeo | **Poppins Bold** | 700 | Rótulos y subtítulos de reels |

**Patrón de marca:** titular en serif con **una palabra en cursiva y color acento**, como en «Los 200 € *escondidos*», donde *escondidos* va en cursiva caramelo.

> ⚠️ **Incoherencia a resolver:** la web usa Instrument Serif y el ebook y el perfil usan Lora. Recomendación: unificar en **Lora** para que portada, perfil y web compartan el mismo «200».

### Escala (web)
- H1: serif, `clamp(44px, 7vw, 88px)`, interlineado 1.0, tracking −1 %
- H2: serif, 40–56 px
- Cuerpo: Inter 17–18 px, interlineado 1.6
- Etiquetas/badges: Inter 600, 12–13 px, MAYÚSCULAS, tracking +8 %

---

## 4. Estilo visual

### Web y redes (modo oscuro)
- Fondo casi negro con **halo verde muy tenue** detrás del elemento principal
- Bordes redondeados: `22px` en tarjetas y `999px` en pills y botones
- Bordes de 1 px semitransparentes, sin sombras duras
- Ancho máximo de contenido: `1180px`
- Elementos 3D sutiles (Three.js) solo como decoración, nunca para transmitir información
- Animaciones de entrada suaves: aparecer y subir 20–40 px

### Ebook (modo crema)
- Fotografía cálida y natural: madera, manos, bote de monedas, cuaderno
- Cajas «Haz esto hoy» en salvia pálida
- Tablas sencillas, con numeración grande en serif

### Vídeo (reels)
- Estética cinematográfica: luz cálida de lámpara + toques verde azulado, poca saturación
- Planos faceless: manos, móvil, tickets, portátil, personas de espaldas o en perfil
- Subtítulos en Poppins Bold blanco con contorno negro; la palabra que suena, en `#A3D9A5`
- Tarjeta «DI ESTO» crema (`#F7F0E3`), con etiqueta caramelo, para las frases clave
- Cierre fijo: fondo `#08090C` + portada real + pill verde «Ebook PDF · 9,99 €» + «Enlace en mi perfil»
- Audio normalizado a −14 LUFS

### Foto de perfil
- «200» en Lora cremoso que se hunde en una ranura verde, con un € debajo
- Versión principal en fondo oscuro, con alternativas crema y oliva

---

## 5. Tono de voz

**Cómo hablamos:**
- De **tú**, cercano, frases cortas.
- Concreto: tareas, minutos, guiones. Nada de teoría abstracta.
- Honesto: «depende de tus gastos actuales», «es un potencial, no una promesa».
- Sin dramas ni culpa: el problema no es la persona, es que nadie le enseñó a mirar sus gastos.
- Español de España: «móvil», «portabilidad», «compañía», «a fin de mes», «tarifa».

**Cómo NO hablamos:**
- ❌ «Hazte rico», «libertad financiera en 30 días», «ingresos pasivos»
- ❌ Testimonios, cifras o descuentos inventados
- ❌ Urgencia falsa («solo hoy», «últimas plazas»)
- ❌ Jerga de inversión, criptomonedas o trading

| En vez de… | Decimos… |
|---|---|
| «Ahorra 200 € garantizados» | «Busca los 200 € que se te escapan cada mes» |
| «Método secreto» | «Un plan de 30 días, 15 minutos al día» |
| «Cambia tu vida» | «Empieza a cambiar tu relación con el dinero» |

---

## 6. Frases de marca (en uso)

**Web**
- «Tu dinero puede hacer mucho más. Aprende a gestionarlo.»
- «¿Trabajas, cobras y no sabes dónde acaba tu dinero?»
- «Empieza a cambiar tu relación con el dinero.»
- «Un plan claro, semana a semana.»
- «Míralo por dentro antes de comprar.»
- «Antes de decidir.»
- «El mejor momento para empezar a gestionar mejor tu dinero es ahora.»

**Ebook**
- «Plan de 30 días para encontrar dinero en tus gastos sin renunciar a nada»
- «Escrito por alguien que ha estado en tu situación»
- Método en 4 pasos: **Mira · Recorta · Tapa · Automatiza**
- «Haz esto hoy»

**Reels**
- «Esta frase puede bajarte la factura del móvil en una sola llamada.»
- «Estoy contento con el servicio, pero he encontrado lo mismo por tanto al mes. Antes de pedir la portabilidad, ¿podéis mejorarme el precio?»
- «Sin dramas.»
- «Tengo este guion y cinco más… en la guía de mi perfil.»

**Bio**
- «Ahorro doméstico en España · Trucos para pagar menos · Reto de 30 días»

**Badges**
- Acceso inmediato · Pago único · Reto de 30 días · 15 min al día · Guiones incluidos

**CTA**
- «Quiero la guía →» (recomendado como **único** CTA principal)

> ⚠️ **Incoherencia a resolver:** la web tiene 4 CTA distintos («Quiero tomar el control de mi dinero», «Quiero la guía», «Quiero mi ebook», «Empieza hoy»). Repetir el mismo texto refuerza la acción: usa «Quiero la guía →» en todos y deja «Empieza hoy →» solo para el cierre.

> ⚠️ **Tono a revisar:** el hero actual («Tu dinero puede hacer mucho más») es genérico y vale para cualquier marca de finanzas. El de la cuenta es más concreto y propio: «¿Dónde se van tus 200 € al mes?».

---

## 7. Aviso legal (obligatorio en piezas largas)
> Contenido educativo y general. No es asesoramiento financiero, legal ni fiscal personalizado. Los resultados dependen de tus gastos actuales. Precios y condiciones pueden cambiar.

---

## 8. Datos del producto

| | |
|---|---|
| Producto | Ebook PDF «Los 200 € escondidos» |
| Precio | 9,99 € (IVA incluido, pago único) |
| Plataforma | Hotmart |
| Enlace de pago | `https://go.hotmart.com/U108442217R?dp=1` |
| Web | `https://200escondidos.pages.dev` |
| Instagram | `@los200escondidos` |

---

## 9. Pendiente de completar (Instagram)
Instagram no permite leer el perfil de forma automática. Para cerrar este documento, añade:
- [ ] Captura de la cuadrícula (los 9 últimos posts) → estilo de portadas de reels
- [ ] Nombre visible y bio actual
- [ ] Destacados (nombres y portadas)
- [ ] Hashtags que usas habitualmente

---

## 10. Checklist rápido para cualquier pieza nueva
- [ ] ¿Usa solo una de las dos paletas (oscura o crema), sin mezclarlas?
- [ ] ¿El verde se usa solo para la acción o el dinero?
- [ ] ¿Titular en serif con una palabra en cursiva y acento?
- [ ] ¿Habla de tú, en concreto y sin prometer cifras?
- [ ] ¿Se entiende sin sonido (subtítulos o rótulos)?
- [ ] ¿El CTA es «Quiero la guía →» o «Enlace en mi perfil»?
- [ ] ¿Sin testimonios, descuentos ni urgencias inventadas?
