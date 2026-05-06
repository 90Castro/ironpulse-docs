# PROJECT STATE — Estado actual de los proyectos

> **Propósito:** foto actual del estado de cada proyecto.
> **Se actualiza tras cada sesión** sustituyendo la información obsoleta.
> Histórico completo en `PROJECT_LOG.md`.

---

## 🟢 PROYECTO ACTIVO: IronPulse (smartwatches)

### Estado general
- **Fase:** catálogo importado en AutoDS (5/5 SKUs como borrador). Pendiente renombrar, copy honesto, imágenes Photoroom y publicar en Shopify.
- **Deadline de lanzamiento:** semana del 4-10 de mayo de 2026.
- **Mercados:** EEUU + Europa, ambos abiertos.
- **Modelo de negocio:** tienda multimarca con curación (retailer) bajo nombres comerciales propios IronPulse.
- **Principio rector:** honestidad por encima de marketing inflado. Las fichas en tienda reescriben las specs reales y añaden sección "Lo que NO tiene" cuando el listing del proveedor infla las características.

### Decisiones cerradas

| Tema | Decisión |
|---|---|
| Marca | IronPulse |
| Dominio | ironpulsewatch.com (registrado, expira 20/04/2027, configurado en Shopify) |
| Plataforma | Shopify "Pulso de Hierro" (admin.shopify.com/store/na111s-jh) |
| Tema | Dawn (gratuito) |
| Proveedor | AliExpress Official Stores / Marcas+ |
| Apps de dropshipping | DSers-AliExpress + AutoDS instaladas |
| Herramienta de imagen | Photoroom (IA, conectada a Shopify) |
| Mercado | EEUU + Europa |
| Idioma | Inglés |
| Logo | Montaña + rosa de los vientos (elegido, pendiente preparar versiones) |

### Estado de plataformas verificado (06/05/2026)
- **Shopify:** logueado, dominio configurado, 0 productos cargados, 0 de 7 tareas de configuración inicial completadas.
- **DSers-AliExpress:** instalada.
- **AutoDS:** Plan Básico 500 ($39,90/mes) — **5/5 SKUs importados como borrador, 0 publicados en Shopify**. Uso: 5/500 variaciones, 1/1 tienda.
- **Google Drive:** Documento Maestro y "IronPulse — Catálogo SKUs v1" accesibles.
- **Limitación conocida:** la skill de Shopify NO permite subir imágenes de producto con fiabilidad — esa tarea la ejecuta siempre Antonio a mano.

### Catálogo definitivo (5 SKUs)

Salto de precio diseñado para que cada gama tenga hueco emocional y funcional propio: **60 → 80 → 120 → 150 → 250 EUR**.

| Nombre comercial | Modelo proveedor | Vendedor AliExpress | Almacén | PVP | Posicionamiento |
|---|---|---|---|---|---|
| **IronPulse Recon** | ChiBear H16 | ChiBear Watch Store (Marcas+, NO Brand Verified) | Choice ES | 59,99 EUR | Entrada táctica |
| **IronPulse Field** | HAYLOU Iron Neo (2025) | Haylou Europe Store (Official, Marcas+) | Germany | 79,99 EUR | Básico fiable |
| **IronPulse Trail** | NORTH EDGE Cross Fit 3 | NORTH EDGE Smartwatch Store (Official) | Choice ES | 119,99 EUR | Outdoor con GPS real |
| **IronPulse Edge** | Zeblaze Stratos 3 Pro | Zeblaze Official Store | EU + US (variantes) | 149,99 EUR | Premium GPS+AMOLED validado |
| **IronPulse Ultra** | Kospet Tank T3 Ultra 2 | kospet Official Store (Marcas+ Verificado) | Local+ US + Brand+ EU | 249,99 EUR / 229,99 USD | Tope rugged 5ATM IP69K |

### URLs de proveedor (ID AliExpress)
- Recon: 1005007224058908 (es.aliexpress.com)
- Field: 1005009552458449 (es.aliexpress.com)
- Trail: 1005005495407391 (es.aliexpress.com)
- Edge: 1005006786664858 (es) / 3256806600350106 (us)
- Ultra: 1005008454557604 (es) / 3256808268242852 (us)

### Estado real en AutoDS tras importación (06/05/2026)

Los 5 SKUs están como borrador en AutoDS con título genérico de AliExpress (renombrar pendiente). PVP cargado correctamente según catálogo:

| Cat. | Título actual en AutoDS | PVP | Ganancia | Almacén usado | Notas |
|---|---|---|---|---|---|
| Recon | "Nuevo reloj inteligente GPS militar… 600 mAh" | 23,85 - 59,99 € | 4,11 - 39,24 € | (revisar) | 6 variantes EN STOCK. Margen mínimo 4,11 € peligroso — auditar variantes. |
| Field | "Reloj inteligente IRON NEO 1,95'' 3 ATM" | 79,99 € | 61,90 € | Porcelana (CN) | Importado con almacén CN; cambiar a Alemania según catálogo. Margen 77%. |
| Trail | "Nuevo reloj GPS… AMOLED 50m ATM, altímetro/barómetro" | 119,99 € | 77,76 € | (revisar) | Margen 65%. |
| Edge | "[Estreno mundial 2024] Stratos 3 Pro AMOLED 1,43''" | 149,99 € | 104,66 € | (revisar) | Margen 70%. |
| Ultra | "TANK T3 Ultra 2 GPS IP69K AMOLED" | 249,99 € | 131,59 € | EEUU | Margen 53%. Antonio cambió almacén a EEUU para sortear bloqueo "ALL". |

### Hallazgos técnicos de AutoDS (06/05/2026)
- **Bloqueo "Envío a ALL"**: AutoDS valida que el listing sea capaz de enviar a "ALL" países. Si la variante por defecto del producto en AliExpress no envía a algún destino global, el botón "Publicar en la tienda" y "Agregar como borrador (página simple)" disparan error toast: *"Envío no disponible para la región seleccionada. No pudimos importar este producto porque actualmente no está disponible para envío desde el almacén en [CN/DE/EE.UU.] a ALL"*.
- **Bypass conocido**: el botón naranja **"Edita la página del producto con IA"** crea un pre-borrador sin validar destino "ALL" y sin gastar créditos (cancelar el modal de upsell de IA mantiene el borrador creado).
- **Solución alternativa (la que usó Antonio para el Ultra)**: cambiar el desplegable "Envío desde almacén" antes de pulsar el botón de import, eligiendo un almacén que sí envíe a "ALL" (en el caso del Ultra, Estados Unidos).
- **Configuración global de destinos**: la URL `/auto-ordering-settings` y `/settings/shipping` redirigen a `plansAddons` en el plan Básico 500. Solo se accede desde el toast de error cuando aparece la frase "consulta tu configuración de envío" — botón que se cierra muy rápido.

### Notas de verificación de listings (30/04/2026)
- **Field (HAYLOU Iron Neo):** coste 27,39 EUR, próximo precio anunciado 20,99 EUR. Subida desde 20,79 EUR (28/04). Recalcular margen al PVP 79,99 EUR antes de carga definitiva.
- **Edge (Zeblaze Stratos 3 Pro):** coste 46,19 EUR, próximo precio 42,14 EUR. Modelo más validado del catálogo: 565 valoraciones, 2.000+ vendidos.
- **Ultra (Kospet Tank T3 Ultra 2):** coste 140,69 EUR (-50% dto. de 281,38 EUR). Subida fuerte respecto al 28/04 (era 119,99 USD ≈ 110 EUR). Final de promo Día de la Madre afecta al margen — prioridad recalcular antes de lanzar.
- **Trail (NORTH EDGE Cross Fit 3):** coste 55,99 EUR (próximo 52,39 EUR). 75 vendidos, 4★. AMOLED + GPS confirmados.
- **Recon (ChiBear H16):** no se pudo reverificar listing concreto desde búsqueda genérica. Notas operativas siguen siendo las del Catálogo SKUs v1.
- **Stock Ultra US (Local+):** no verificable desde sesión geo-fijada a España. PENDIENTE para Antonio en sesión .com con dirección US.
- **Implicación general:** las ofertas Día de la Madre están cayendo. Costes reales post-promo subirán los márgenes calculados el 28/04 en 5-15 EUR por unidad. Antes de carga definitiva, recalcular margen con coste actual o esperar a estabilización.

### SKU descartado: M99 SIM 4G (29/04/2026)
- Producto OEM genérico chino rebadgeado (GOLDENSPIKE, XINDADA, iMosi, EDMUND).
- Mentiras del listing: "5G" (es 4G Cat-4), RAM 32GB y ROM 512GB (imposibles), batería 2100 mAh (real ~700-900 mAh, autonomía 24-36h confirmada por review independiente).
- Vendedor no oficial, garantía cumple solo 43% según valoraciones.
- **Decisión:** descartado. No cumple el principio de honestidad y rompería el ADN deportivo/rugged del catálogo.
- **Búsqueda SIM 4G aplazada a v2 del catálogo.** Candidato a reevaluar: Kospet iHeal 5 / Optimus 3 (misma familia que Ultra → comparten marca y soporte postventa).

### Política de transparencia de marca
**Decisión:** Opción B con mitigaciones — la marca del fabricante aparece únicamente en el desplegable "Technical Specifications".

**Formato estándar de especificaciones técnicas (todos los SKUs):**
```
▼ TECHNICAL SPECIFICATIONS
Manufacturer: [ChiBear / Haylou / North Edge / Zeblaze / Kospet]
Model: [modelo real]
Display: [...]
Water resistance: [...]
Battery: [...]
[resto de specs reales del producto]

Curated and serviced by IronPulse.
```

**Mitigaciones obligatorias:**
- Email post-compra menciona el fabricante real.
- Política de devoluciones: 30 días sin preguntas, gastos pagados.
- Reserva económica: 5-10% de cada venta para devoluciones/chargebacks.
- Pasarelas: Shopify Payments + PayPal como respaldo.
- KPIs de alarma: >2% chargebacks o reseñas negativas con mención de marca → activar plan B (cambio a Opción D, marca visible).

### Reglas de presentación en tienda
1. Copy honesto en TODOS los SKUs. Especialmente crítico en Recon: sección "Lo que NO tiene" obligatoria.
2. Marca proveedor (ChiBear, Haylou, North Edge, Zeblaze, Kospet) NO se expone como rótulo principal. Solo el nombre comercial IronPulse.
3. Argumento "envío rápido US" SOLO se promete en Edge y Ultra (almacén US confirmado). En Recon/Field/Trail se declara honestamente "Ships from EU — 5 to 13 business days" para clientes US.
4. Geo-routing en Shopify: aplicar por SKU según disponibilidad geo verificada.

### Riesgos legales asumidos por Antonio (decisión informada)
- IRONPULSE registrada en Francia por CONCEPT LABEL SAS (clase de ropa/accesorios/deporte) y en uso comercial activo en Amazon ES/FR/BE/IT/MX para chalecos lastrados.
- Existencia de Iron Pulse LLC en EEUU con solicitud pendiente en Clase 9 (24 dic 2025) que cubre smartwatches.
- Riesgos de Opción B de transparencia (Directiva 2005/29/CE de prácticas comerciales desleales).

### Plan de contingencia C&D (acordado)
Si llega cualquier indicio real de problema (carta C&D, queja formal, retirada por plataforma, denuncia, requerimiento legal):
1. Se cierra inmediatamente la tienda afectada.
2. Se conserva el inventario digital, fotos y aprendizajes operativos.
3. Se relanza con marca y dominio nuevos (no relacionados) y, si procede, con productos diferentes.
4. No se contesta a la C&D sin haber consultado primero a un abogado de marcas.

Mientras no llegue ningún indicio real, se vende con normalidad y se prioriza facturación.

### Copy honesto definitivo (redactado 30/04/2026)
Borrador completo de las 5 fichas Shopify ya redactado y disponible en el documento operativo "IronPulse — Catálogo SKUs v1" (Google Drive). Pendiente de revisión final de Antonio antes de cargar.

### Trabajo pendiente (orden propuesto tras sesión 06/05/2026)
1. **Auditar variantes y márgenes del Recon** — el rango 4,11 € - 39,24 € indica que alguna variante (probablemente "malla negro" o "acero negro") tiene coste muy alto. Decidir variantes vivas o subir PVP de las caras.
2. **Ajustar almacén del Field a Alemania** en AutoDS (ahora está en Porcelana/CN; el catálogo manda Germany para envíos rápidos a EU).
3. **Verificar stock Ultra US (Local+)** desde sesión .com con dirección de EE.UU. (tarea de Antonio).
4. **Renombrar títulos** de los 5 productos a la convención IronPulse (Recon, Field, Trail, Edge, Ultra).
5. **Recalcular márgenes** con costes post-promo Día de la Madre antes de publicar.
6. **Revisar copy honesto** de las 5 fichas (ya redactadas en el doc operativo).
7. **Trabajar imágenes en Photoroom** para los 5 SKUs (subida manual la hace Antonio).
8. **Configurar variantes invisibles** del Ultra: Alemania para Europa, Estados Unidos para América.
9. **Publicar productos** en Shopify (5 SKUs) desde AutoDS.
10. **Configuración Shopify (sesión siguiente):** pasarelas de pago (Shopify Payments + PayPal); páginas legales (aviso legal, política de privacidad, términos, envíos, devoluciones); zonas de envío EU + US y reglas de geo-routing por SKU; impuestos (IVA EU + sales tax US según estado).
11. **Preparar versiones del logo** (fondo transparente, blanco, solo ícono, favicon).

---

## 🟡 PROYECTO EN ESPERA: PLAYBACK Store (retro/nostalgia)

### Estado general
- **Fase:** investigación pausada hasta lanzar IronPulse.
- **Concepto:** tienda online retro/nostalgia 80-90 con foco en música y gaming de la generación que hoy tiene 30-40 años. Identidad emocional fuerte, no commodity.
- **Mercado inicial:** solo España.
- **Cliente objetivo:** españoles de 28-45 años con poder adquisitivo medio que vivieron casete → CD → MP3 y Game Boy/PlayStation. "El cliente es Antonio hace 20 años."

### Mercado validado
- Ventas de casetes **+204,7% Q1 2025** en Europa (63.288 unidades).
- 59% de la Gen Z escucha formatos físicos.
- Marca francesa "We Are Rewind" vende reproductores de casete a 149€ → valida que hay demanda y precio alto dispuesto a pagarse.

### Decisiones cerradas

| Tema | Decisión |
|---|---|
| Modelo | Dropshipping puro, sin stock |
| Marca | PLAYBACK Store |
| Tagline candidato | "Dale al play a tus recuerdos" / "Algo con alma" |
| Plataforma | Shopify (plan Basic mensual) |
| Proveedor principal (fase 1) | CJdropshipping (cuenta creada) |
| Proveedor de calidad (fase 2) | Spocket |
| Proveedor escalado (fase 3) | BigBuy |
| Apps Shopify | DSers/CJdropshipping (gratis), Vitals (~29€/mes), Translate & Adapt (gratis) |
| Estrategia de pagos | Shopify Payments para evitar comisión adicional |
| Dominio | playbackstore.es (comprado) |

### Identidad visual

**Paleta de colores PLAYBACK Store v2:**

| Nombre | Hex |
|---|---|
| Crema foto | #FAF6EE |
| Arena cálida | #EDE3D5 |
| Ámbar suave | #E8C9A0 |
| Terracota 90 | #A0736B |
| Azul cielo | #A8C4CC |
| Verde pastel | #C4D4A8 |
| Marrón texto | #5C4A35 |

- **Logo:** "PLAYBACK ▸ STORE · EST. 2025" en marrón texto sobre fondos crema/arena/azul.
- **Estética:** foto revelada en laboratorio del barrio. Tonos cálidos desteñidos.

### Estrategia de contenido
- **Plataformas:** TikTok + Instagram Reels + YouTube Shorts.
- **Cuentas a reservar:** @playbackstore en las tres redes.
- **Frecuencia:** 3 vídeos/semana.
- **Producción:** todo con IA. Antonio escribe los guiones (con ayuda), las voces, subtítulos y vídeo se generan con IA. No quiere aparecer en cámara.
- **Reciclaje:** un vídeo, tres redes (sin triplicar el trabajo).

### Stack de IA para contenido (cerrado)

| Función | Herramienta | Coste |
|---|---|---|
| Guiones | Claude | en uso |
| Generación de vídeo (principal) | InVideo AI | ~20€/mes (Pro) |
| Generación con avatar (fase 2) | HeyGen | ~29$/mes cuando aplique |
| Edición y subtítulos | CapCut | Gratis |
| Programación multi-red | Metricool | Gratis |

**Coste mensual estimado del stack de contenido:** ~20€.

### Riesgos vivos
- 14 registros activos en clases 9/35 con conflictos parciales (PLAYBACK SL Madrid en clase 35 limitada a moda; Playback Store Medellín Colombia con presencia en redes). Antonio asume el riesgo.

### Trabajo pendiente (cuando se reactive)
1. Verificar marca PLAYBACK en OEPM/EUIPO/TMView clases 9 y 35.
2. Reservar redes sociales aunque no se publique aún.
3. Cerrar catálogo definitivo (búsqueda conjunta en CJ/Spocket/AliExpress ES).
4. Crear cuenta Shopify y aplicar identidad visual.
5. Escribir guión del primer vídeo TikTok.

---

## 📋 PRÓXIMA SESIÓN — AGENDA

**Fecha objetivo:** 07/05/2026 y siguientes.

**Objetivo único de la sesión:** dejar las fichas IronPulse listas en AutoDS (variantes, almacén correcto, títulos IronPulse, copy honesto e imágenes Photoroom) y publicar los 5 SKUs en Shopify.

**Antonio llega con:**
- Imágenes base de los 5 SKUs ya editadas en Photoroom (fondo limpio, vista principal mínimo + lateral si es posible).
- Cuenta Shopify y AutoDS accesibles y con sesión iniciada.
- Doc "IronPulse — Catálogo SKUs v1" abierto.
- Verificación de stock Ultra US (Local+) desde sesión .com con dirección US (si la tiene hecha).
- Al menos 3 horas reservadas para trabajar continuado.

**Plan de trabajo en sesión:**
1. Auditar variantes Recon y decidir cuáles dejar vivas / ajustar PVP.
2. Cambiar almacén del Field a Alemania en AutoDS.
3. Renombrar los 5 SKUs a "IronPulse Recon / Field / Trail / Edge / Ultra".
4. Recalcular márgenes finales con costes actualizados.
5. Aplicar copy honesto desde el doc operativo (descripciones, viñetas, sección "Lo que NO tiene" en Recon).
6. Configurar variantes invisibles del Ultra (Alemania=EU, EEUU=US).
7. Publicar los 5 SKUs en Shopify desde AutoDS.
8. Dejar la lista de tareas pendientes para la sesión siguiente (configuración Shopify: pasarelas, legales, envíos, impuestos).

**Tareas que NO entran en esta sesión** (van a la siguiente): pasarelas de pago, páginas legales, configuración fiscal, geo-routing avanzado, lanzamiento.
