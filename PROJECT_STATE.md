# PROJECT STATE — Estado actual de los proyectos

> **Propósito:** foto actual del estado de cada proyecto.
> **Se actualiza tras cada sesión** sustituyendo la información obsoleta.
> Histórico completo en `PROJECT_LOG.md`.

---

## 🟢 PROYECTO ACTIVO: IronPulse (smartwatches)

### Estado general (actualizado 08/05/2026)

- **Fase:** **ONE-PRODUCT STORE en lanzamiento** — IronPulse Edge creado en Shopify como producto activo (pendiente solo subir imágenes Photoroom).
- **Estrategia:** lanzamiento como tienda mono-producto con el Edge (Zeblaze Stratos 3 Pro) como único SKU activo. Recon/Field/Trail/Ultra permanecen como borradores en AutoDS, en stand-by para Fase 2/3.
- **Razón del pivote:** maximizar foco, simplicidad operativa y curva de aprendizaje en una primera tienda. Activar resto del catálogo solo cuando haya datos de validación del Edge.
- **Mercados:** EU activo (Phase 1). US queda para Phase 1.5 cuando se confirme almacén US.
- **Modelo de negocio:** retailer dropshipping bajo nombre comercial propio IronPulse.
- **Principio rector:** honestidad por encima de marketing inflado. Sin promesas falsas de envío rápido US mientras solo opere EU.

### Plan de fases (actualizado 07/05/2026)

| Fase | Periodo | Acción |
|---|---|---|
| Fase 1 | Mes 1-2 | Lanzamiento y validación del Edge (one-product store) |
| Fase 1.5 | Mes 1-2 | Activar almacén US en Edge cuando esté validado el flujo EU |
| Fase 2 | Mes 2-3 | Si vende, añadir Ultra como anchor premium |
| Fase 3 | Mes 3+ | Activar Recon/Field/Trail como upsell/downsell |

### Decisiones cerradas

| Tema | Decisión |
|---|---|
| Marca | IronPulse |
| Dominio | ironpulsewatch.com (registrado, vence 20/04/2027, configurado en Shopify) |
| Plataforma | Shopify "Iron Pulse" (admin.shopify.com/store/na111s-jh) |
| Tema | Dawn (gratuito) |
| Proveedor | AliExpress Official Stores / Marcas+ |
| Apps de dropshipping | DSers-AliExpress + AutoDS instaladas |
| Herramienta de imagen | Photoroom (IA, conectada a Shopify) |
| Mercado activo | EU (US en Phase 1.5) |
| Idioma | Inglés |
| Logo | Montaña + rosa de los vientos (elegido, pendiente preparar versiones) |
| Modelo de tienda | One-product store (Phase 1) |
| Producto activo | IronPulse Edge (Zeblaze Stratos 3 Pro) |

### IronPulse Edge — ESTADO EN SHOPIFY (creado 08/05/2026)

URL admin: `/store/na111s-jh/products/15494238896505`

| Campo | Valor |
|---|---|
| Título | IronPulse Edge — AMOLED + GPS, validated by thousands |
| Descripción | Copy honesto en inglés (1509 chars) — bloques *What it does*, *Real validation*, *Shipping*, *Returns* y dropdown *Technical Specifications* |
| Tagline de marca | "The smartwatch built for those who don't stop." |
| PVP | 149,99 € (ambas variantes) |
| Variantes | Color → Ember Black, Ocean Blue |
| Inventario | Sin seguimiento en ambas variantes (sellable, AutoDS gestionará stock) |
| Categoría | Relojes inteligentes en Joyería (+10 metafields auto) |
| Vendor | Iron Pulse |
| Estado | Activo |
| Canales | Tienda online · Shop · Point of Sale |
| Multimedia | **PENDIENTE** — Antonio sube imágenes Photoroom manualmente |

### Criterios por los que se eligió el Edge como SKU único

- Vendedor Zeblaze Official Store (verificado, sin riesgo)
- 565 valoraciones / 2.000+ vendidos (el más validado del catálogo)
- AMOLED + GPS reales (sin discrepancias con la ficha)
- Almacén EU + US disponibles (US para Phase 1.5)
- Margen ~104€ por venta al PVP 149,99€
- Sweet spot de precio (ni barato genérico, ni premium asustando)

### Catálogo en stand-by (Fase 2/3) — borradores intactos en AutoDS

| Cat. | Modelo proveedor | Vendedor AliExpress | PVP previsto | Fase activación |
|---|---|---|---|---|
| Recon | ChiBear H16 | Tienda de relojes ChiBear (Marcas+) | 59,99 € | Fase 3 |
| Field | HAYLOU Iron Neo (2025) | Tienda Haylou Europa (Oficial, Marcas+) | 79,99 € | Fase 3 |
| Trail | NORTH EDGE Cross Fit 3 | NORTH EDGE Smartwatch Store (Official) | 119,99 € | Fase 3 |
| Edge | Zeblaze Stratos 3 Pro | Zeblaze Official Store | **149,99 €** | **ACTIVO Fase 1** |
| Ultra | Kospet Tank T3 Ultra 2 | Kospet Official Store (Marcas+ Verificado) | 249,99 € / 229,99 USD | Fase 2 |

**Regla operativa:** NO tocar Recon/Field/Trail/Ultra en AutoDS hasta validar el Edge. Permanecen como borradores con título genérico de AliExpress.

### Estado de plataformas verificado (08/05/2026)

- **Shopify:** logueado, dominio configurado, **1 producto activo (Edge)**, pendiente subir imágenes y configurar pasarelas.
- **DSers-AliExpress:** instalado.
- **AutoDS:** Plan Básico 500 ($39,90/mes) — 5/5 SKU importados, **1/5 publicado en Shopify (Edge, manualmente — NO via AutoDS)**. Uso: 5/500 variaciones, 1/1 tienda.
- **Conexión AutoDS↔Shopify:** identificado problema en sesión 08/05/2026 — AutoDS muestra "Crea una tienda Shopify" que abre ZipStore externo en lugar de detectar la tienda existente. La app AutoDS sí está instalada en el sidebar de Shopify. **Pendiente reconectar OAuth en próxima sesión** para poder publicar el resto desde AutoDS.
- **Google Drive:** Documento Maestro y "IronPulse — Catálogo SKUs v1" accesibles.

> **Limitación conocida:** la habilidad de Shopify NO permite subir imágenes de producto con confiabilidad — esa tarea la ejecuta siempre Antonio a mano.

### Política de transparencia de marca

**Decisión:** Opción B con mitigaciones — la marca del fabricante aparece **únicamente en el desplegable "Technical Specifications"**.

Aplicado en el Edge en Shopify:

```
▼ TECHNICAL SPECIFICATIONS
Manufacturer: Zeblaze
Model: Stratos 3 Pro
Display: 1.43" AMOLED HD
[resto de specs reales]

Curated and serviced by IronPulse.
```

**Mitigaciones obligatorias:**

- Email post-compra menciona el fabricante real.
- Política de devoluciones: 30 días sin preguntas, gastos pagados.
- Reserva económica: 5-10% de cada venta para devoluciones/chargebacks.
- Pasarelas: Shopify Payments + PayPal como respaldo (PENDIENTE configurar).
- KPIs de alarma: >2% chargebacks o reseñas negativas con mención de marca → activar plan B (cambio a Opción D, marca visible).

### Reglas de presentación en tienda

- Copy honesto en TODAS las fichas. En Edge: sin sección "Lo que NO tiene" porque las specs del proveedor son reales y verificadas.
- Marca proveedor (Zeblaze) NO se expone como rótulo principal. Solo el nombre comercial IronPulse.
- En Phase 1: shipping declarado honestamente "Ships from EU — 5 to 12 business days". US se atiende como "Ships from EU — 8 to 15 business days" hasta activar almacén US.
- Geo-routing en Shopify: por configurar cuando se active US (Phase 1.5).

### Riesgos legales asumidos por Antonio (decisión informada)

- IRONPULSE registrada en Francia por CONCEPT LABEL SAS (clase ropa/accesorios/deporte) en uso en Amazon ES/FR/BE/IT/MX para chalecos lastrados.
- Existencia de Iron Pulse LLC en EEUU con solicitud pendiente Clase 9 (24/12/2025) que cubre smartwatches.
- Riesgos de Opción B de transparencia (Directiva 2005/29/CE de prácticas comerciales desleales).

### Plan de contingencia C&D (acordado)

Si llega cualquier indicio real de problema (carta C&D, queja formal, retirada por plataforma, denuncia, requerimiento legal):

1. Se cierra inmediatamente la tienda afectada.
2. Se conserva el inventario digital, fotos y aprendizajes operativos.
3. Se relanza con marca y dominio nuevos (no relacionados) y, si procede, con productos diferentes.
4. No se contesta a la C&D sin haber consultado primero a un abogado de marcas.

Mientras no llegue ningún indicio real, se vende con normalidad y se prioriza facturación.

### Trabajo pendiente inmediato (después de subir imágenes Edge)

1. **Antonio sube imágenes Photoroom** del Edge en sección Multimedia de Shopify (Ember Black + Ocean Blue + ángulos/lifestyle).
2. Asignar imagen principal a cada variante (icono junto al nombre de la variante).
3. Verificar listado en `/products` muestra el Edge activo con miniatura.
4. Configurar **home page** de Shopify con Edge como hero único + tagline "The smartwatch built for those who don't stop."
5. Reconectar **AutoDS↔Shopify** (OAuth desde el lado de AutoDS) para poder gestionar inventario/pedidos del Edge desde AutoDS.

### Trabajo pendiente sesión siguiente

1. **Pasarelas de pago:** activar Shopify Payments + PayPal.
2. **Páginas legales:** aviso legal, política de privacidad, términos, política de envíos, política de devoluciones (30 días).
3. **Zonas de envío EU:** configurar tarifas (gratis o coste fijo bajo) para todos los países EU activos.
4. **Impuestos:** IVA EU según régimen del vendedor.
5. **Email post-compra:** plantilla con mención al fabricante real (Zeblaze).
6. **Phase 1.5:** activar almacén US en el Edge cuando esté validado el flujo EU + configurar sales tax US según estado.
7. **Marketing inicial:** primeras campañas (creatives en Photoroom + tagline definitiva).
8. **Versiones del logo:** fondo transparente, blanco, solo ícono, favicon.

### Hallazgos técnicos relevantes (mantenidos de sesiones anteriores)

- **Bloqueo "Envío a ALL" en AutoDS:** valida que el listing pueda enviar a "ALL" países; bypass usando "Edita la página del producto con IA" (cancelar el modal upsell mantiene el borrador).
- **AutoDS — edición de descripción:** "solo disponible en versión de escritorio" — descartado en sesión 08/05/2026, descripciones se editan directamente en Shopify.
- **Shopify — campos en Shadow DOM:** los inputs de título usan web components `s-internal-text-field`. Acceso via `titleField.shadowRoot.querySelector('input')` y disparar eventos `input`/`change`.
- **Shopify — descripción:** TinyMCE en iframe `product-description-ro_ifr`. Set `contentDocument.body.innerHTML` y disparar `input` en el body.
- **Cuidado con CTRL+K:** typear "—" en contexto sin foco activa la barra de búsqueda global de Shopify y puede navegar a páginas no deseadas.
- **Stock Ultra US (Local+):** no verificable desde sesión geo-fijada a España. Pendiente para Antonio en sesión .com con dirección US (relevante solo cuando se active Fase 2).

---

## 🟡 PROYECTO EN ESPERA: PLAYBACK Store (retro/nostalgia)

### Estado general

- Fase: investigación pausada hasta lanzar IronPulse.
- Concepto: tienda online retro/nostalgia 80-90 con foco en música y gaming de la generación que hoy tiene 30-40 años. Identidad emocional fuerte, no commodity.
- Mercado inicial: solo España.
- Cliente objetivo: españoles de 28-45 años con poder adquisitivo medio que vivieron casete → CD → MP3 y Game Boy/PlayStation. "El cliente es Antonio hace 20 años."

### Mercado validado

- Ventas de casetes +204,7% Q1 2025 en Europa (63.288 unidades).
- 59% de la Gen Z escucha formatos físicos.
- Marca francesa "We Are Rewind" vende reproductores de casete a 149€ → valida demanda y precio alto dispuesto a pagarse.

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

Paleta de colores PLAYBACK Store v2:

| Nombre | Hex |
|---|---|
| Crema foto | #FAF6EE |
| Arena cálida | #EDE3D5 |
| Ámbar suave | #E8C9A0 |
| Terracota 90 | #A0736B |
| Azul cielo | #A8C4CC |
| Verde pastel | #C4D4A8 |
| Marrón texto | #5C4A35 |

Logo: "PLAYBACK ▸ STORE · EST. 2025" en marrón texto sobre fondos crema/arena/azul.
Estética: foto revelada en laboratorio del barrio. Tonos cálidos desteñidos.

### Estrategia de contenido

- Plataformas: TikTok + Instagram Reels + YouTube Shorts.
- Cuentas a reservar: @playbackstore en las tres redes.
- Frecuencia: 3 vídeos/semana.
- Producción: todo con IA. Antonio escribe los guiones (con ayuda), las voces, subtítulos y vídeo se generan con IA. No quiere aparecer en cámara.
- Reciclaje: un vídeo, tres redes (sin triplicar el trabajo).

### Stack de IA para contenido (cerrado)

| Función | Herramienta | Coste |
|---|---|---|
| Guiones | Claude | en uso |
| Generación de vídeo (principal) | InVideo AI | ~20€/mes (Pro) |
| Generación con avatar (fase 2) | HeyGen | ~29$/mes cuando aplique |
| Edición y subtítulos | CapCut | Gratis |
| Programación multi-red | Metricool | Gratis |

Coste mensual estimado del stack de contenido: ~20€.

### Riesgos vivos

- 14 registros activos en clases 9/35 con conflictos parciales (PLAYBACK SL Madrid en clase 35 limitada a moda; Playback Store Medellín Colombia con presencia en redes). Antonio asume el riesgo.

### Trabajo pendiente (cuando se reactive)

1. Verificar marca PLAYBACK en OEPM/EUIPO/TMView clases 9 y 35.
2. Reservar redes sociales aunque no se publique aún.
3. Cerrar catálogo definitivo (búsqueda conjunta en CJ/Spocket/AliExpress ES).
4. Crea cuenta Shopify y aplica identidad visual.
5. Escribir guión del primer vídeo TikTok.

---

## 📋 PRÓXIMA SESIÓN — AGENDA

**Fecha objetivo:** próxima sesión Antonio.

**Objetivo único:** dejar el IronPulse Edge listo para vender (imágenes + home + pasarelas + legales) y preparar Phase 1.5 (US).

**Antonio llega con:**

- Imágenes Photoroom del Edge ya editadas (Ember Black + Ocean Blue + ángulos + lifestyle).
- Cuenta Shopify y AutoDS accesibles y con sesión iniciada.
- Decisión sobre activación US (¿Phase 1 o esperar a Phase 1.5?).
- Al menos 2-3 horas reservadas para trabajar seguido.

**Plan de trabajo en sesión:**

1. Subir imágenes al Edge en Shopify (Antonio) y asignarlas a variantes.
2. Configurar home page de Shopify: Edge como hero único + tagline "The smartwatch built for those who don't stop."
3. Reconectar AutoDS↔Shopify (OAuth) para gestionar pedidos del Edge desde AutoDS.
4. Activar Shopify Payments + PayPal como pasarelas.
5. Crear páginas legales (aviso legal, privacidad, términos, envíos, devoluciones 30 días).
6. Configurar zona de envío EU con tarifas.
7. Configurar IVA EU.
8. Crear plantilla email post-compra mencionando fabricante real (Zeblaze).
9. Lanzamiento "soft" — pedir feedback a círculo cercano antes de campañas.

**Tareas que NO entran en esta sesión (van a siguientes):** Phase 1.5 (almacén US + sales tax), activar Ultra como anchor (Fase 2), activar Recon/Field/Trail (Fase 3), preparar versiones del logo, primeras campañas de marketing.
