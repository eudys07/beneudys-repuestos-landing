# R&E Beneudys Repuestos — Landing page

Página de presencia de marca para **R&E Beneudys SRL**, repuestos para camiones y
vehículos pesados en Santo Domingo Oeste, República Dominicana.

Sitio estático: un solo `index.html` con el CSS embebido, sin build ni dependencias.

## Estructura

```
index.html                  Página completa (HTML + CSS)
assets/
  logo-white.png            Emblema en blanco, fondo transparente (el que usa la página)
  logo-white-con-rnc.png    Misma versión conservando la línea del RNC
  logo.png                  Render original del emblema, sin modificar
  marcas/                   Logos de Shacman, Sinotruk, Mack y Cummins
docs/superpowers/specs/     Documento de diseño
```

## Ver en local

```bash
python3 -m http.server 8765
```

Luego abrir http://localhost:8765

## Datos de contacto en la página

- Teléfono / WhatsApp: 809-766-4523
- Dirección: Avenida Independencia No. 45, Km 12, Carr. Sánchez, Costa Verde, Santo Domingo Oeste
- Horario: Lunes a Viernes 8:00am–6:00pm · Sábado 8:00am–2:00pm · Domingo cerrado

## Pendiente antes de publicar

- Reemplazar el dominio marcador `beneudysrepuestos.com` en `<link rel="canonical">` y `og:url`.
- Agregar una imagen `og:image` propia para compartir en redes.
- El logo de Sinotruk es el corporativo del grupo (CNHTC); sustituir si se prefiere la variante verde.
