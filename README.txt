DYSONTECH / DYFIX ONE PAGE

REVISIÓN ADICIONAL (checklist unificado de la familia, a petición del cliente — repo 5/48):
- BUG REAL — enlace de Cal.com desactualizado. Actualizado a
  https://cal.com/kelatos/30min?embed=true&theme=light&attendeePhoneNumber=%2B34&overlayCalendar=true.
- Verificado: el correo soporte@kelatos.com no aparece visible.
- BUG REAL — el mensaje prellenado de WhatsApp decía "¡Hola Kelatos!".
  Corregido a "¡Hola DyFix!" en el CTA del hero y en el botón flotante.
- Verificado: el menú móvil (#mainMenu) ya cierra correctamente al
  seleccionar cualquier enlace.
- Verificado: sin iconos ni imágenes con proporciones fijas
  incorrectas.
- BUG REAL — el H1 en móvil estaba en 47px, no en el estándar de 48px
  pedido por el cliente. Corregido a 48px.
- BUG REAL — botones del hero (.cta) con border-radius de 15px y sin
  ningún estado hover. Aumentado a border-radius:999px; añadido
  filter:brightness(.88) en wa/pickup y fondo navy sólido con texto
  blanco en el botón de teléfono al pasar el ratón.
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

REVISIÓN ADICIONAL (checklist unificado de la familia, a petición del cliente):
- H1 repetía la plantilla "no funciona" usada en varios repos.
  Reescrito con estructura de una sola frase, imperativa: "Repara tu
  Dyson en 2 horas, con garantía." (8 palabras).
- BUG REAL — texto decorativo ".fast-art:before" ("2 h", 150px) sin
  reducción de tamaño en móvil/tablet, mismo patrón que ThermomixTech
  y otros repos. Añadida reducción (90px tablet, 56px móvil).
- Enlace de política de privacidad: la casilla existía pero sin
  enlace. Añadido a https://kelatos.com/privacy-policy/, en azul y
  subrayado.
- El aviso de servicio independiente solo estaba en letra pequeña.
  Añadida la franja destacada bajo el menú.
- Añadido "Sábados, domingos y días festivos estamos cerrados" debajo
  del horario.
- Botón "Atención Telefónica..." sin icono, a diferencia del de
  WhatsApp. Añadido.
- Verificado: schema.org ya usaba correctamente el teléfono de la
  caja de información; formulario correctamente conectado a
  /api/contacto. Sin cambios en ninguno de estos.
