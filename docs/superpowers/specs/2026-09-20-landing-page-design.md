# Landing page — R&E Beneudys Repuestos

## Objetivo
Página de presencia de marca en español para "R&E Beneudys SRL" (nombre comercial: "R&E Beneudys Repuestos"), repuestos para camiones y vehículos pesados en Santo Domingo Oeste, República Dominicana. Sin catálogo ni formulario: el objetivo es que el visitante llame o escriba por WhatsApp.

## Marca
- Emblema original en `Emblema_SAMA.pdf`. Derivados en `assets/`:
  - `logo-white.png` — **el que usa la página**: emblema en blanco sobre fondo transparente, **sin la línea del RNC**.
  - `logo-white-con-rnc.png` — misma versión pero conservando el RNC.
  - `logo.png` — render original sin modificar (referencia).
- Paleta: navy `#141d35` / `#0c1224`, blanco, plateado `#c9d1d9`, ámbar `#e8a33d` (acento) y verde WhatsApp `#25d366` (solo para acciones de WhatsApp).
- Tipografía: Inter (Google Fonts).

## Estructura (`index.html`, una sola página)
1. **Header** sticky — emblema 52px, nombre, nav (Marcas / Contacto) y botón WhatsApp (≥720px).
2. **Hero** — emblema 200px sin placa, titular, bajada y dos CTAs (teléfono visible como texto del botón + WhatsApp).
3. **Valores** — tres propuestas: especialización en pesados, atención directa, ubicación.
4. **Marcas** — Shacman, Sinotruk, Mack, Cummins en tarjetas blancas con logo real + nombre.
5. **Contacto** — teléfono, WhatsApp, horario (tabla día/hora) y dirección con enlace "Cómo llegar" a Google Maps.
6. **Footer** — razón social y año. **Sin RNC.**
7. **FAB de WhatsApp** flotante, solo en móvil (<720px).

## Decisiones de UX
- El teléfono aparece como texto del botón principal del hero: en móvil es la acción de mayor intención.
- El emblema se usa con fondo transparente porque su placa navy se fundía con el fondo de la página.
- Los logos de marca van en tarjetas blancas: son multicolor y no se leen sobre navy.
- Caja óptica fija de 72px para los logos, así marcas de distinta proporción pesan igual.
- El horario incluye "Domingo — Cerrado" explícito para evitar el viaje en vano.

## Accesibilidad y SEO
- Skip link, `:focus-visible`, `prefers-reduced-motion`, iconos SVG con `aria-hidden`, secciones con `aria-labelledby`.
- Meta description, Open Graph, `theme-color`, favicon embebido.
- JSON-LD `AutoPartsStore` con teléfono, dirección, horarios y marcas.

## Técnico
- HTML + CSS en un solo archivo, sin build ni JS de aplicación.
- Teléfono: `tel:+18097664523` · WhatsApp: `https://wa.me/18097664523`.
- Vista previa local: `python3 -m http.server 8765` (config en `.claude/launch.json`).

## Pendientes
- Dominio real para `canonical` y `og:url` (hoy `beneudysrepuestos.com` es un marcador).
- Imagen `og:image` propia para compartir en redes.
- Confirmar si se quieren agregar más marcas a la sección.
