DYSONTECH / DYFIX ONE PAGE
Dominio: https://dyfix.eu/
Teléfono caja y botones: +34 910 05 48 17
Diagnóstico: gratuito
Presupuesto: sin compromiso
Garantía: 6 meses
Mensaje de rapidez: Podemos reparar tu Dyson en 2 h, según la avería.
Repara: aspiradoras, Supersonic, Airwrap y purificadores Dyson.
El correo SMTP no aparece visible en la web; solo se usa en /api/contacto.
Variables Vercel compartidas: SMTP_HOST, SMTP_PORT=465, SMTP_SECURE=true, SMTP_USER, SMTP_PASS, CONTACT_EMAIL.
Google Analytics:
G-9WYNNQBCJX

HISTORIAL: el repositorio era multipágina (14 páginas /servicios/ y
/precios/ de reparación y mantenimiento Dyson) y se convirtió a
one-page; esas páginas fueron eliminadas en commits anteriores. Como
ya no existen en el sitemap actual, se ha añadido middleware.mjs para
redirigir (301) cualquier URL antigua a la home, evitando 404 en
enlaces indexados o backlinks antiguos. Excluye /api/* y cualquier
ruta con extensión de archivo. Se añadió "@vercel/functions": "^2.0.3"
a package.json como dependencia de esta función.

NOTA: este es el repositorio original de Madrid del que partió una
copia para crear DysonTech Valladolid (repo DysonValladolid). El
dominio (dyfix.eu) y el teléfono (+34 910 05 48 17) de este repo son
los correctos y de referencia — Valladolid los comparte de forma
intencional, según confirmó el cliente.

REVISIÓN (fixes aplicados en esta pasada):
- Ya estaba bien: sección SEO "Guía" (id="sobre-dyson"), menú móvil,
  borde blanco del chat, api/contacto.js con SMTP + nodemailer,
  dominio ya en https. No se ha modificado ninguno de estos.
- Banner de cookies: no existía (a diferencia del resto de la
  familia). Añadido (Aceptar / Rechazar / Política de privacidad →
  https://kelatos.com/privacy-policy/), con diseño apilado a ancho
  completo en móvil.
- Google Analytics: no existía. Añadido G-9WYNNQBCJX.
- Schema.org: faltaban areaServed y sameAs (Maps/YouTube) — añadidos.
- .navcall: el texto largo ("Atención Telefónica 24 horas 365 días")
  deformaba la píldora del menú. Acortado a solo el número (mismo
  número, +34 910 05 48 17) y añadido white-space:nowrap como
  salvaguarda. El botón grande .cta.phone del hero conserva su texto
  completo.
- H1 de portada reescrito, corto, directo y totalmente afirmativo
  (sin interrogación ni condicionales), incluye la marca y la promesa
  de rapidez ya existente en la web: "Tu Dyson no funciona. Te lo
  devolvemos reparado en 2 horas." Tamaño del H1 aumentado:
  clamp(38-55px) → clamp(46-73px) en escritorio, 39px → 47px en móvil.
