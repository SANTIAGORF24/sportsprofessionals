# 🏟️ Sports Professionals — Sitio corporativo

> Sitio web institucional para una empresa de **administración de escenarios deportivos y
> servicios recreativos**. Next.js con App Router, catálogo dinámico de escenarios y
> contacto directo por WhatsApp.

---

## 🗺️ Secciones

| Ruta | Contenido |
| --- | --- |
| `/` | Portada con slider de banners y servicios destacados |
| `/quienes-somos` | Presentación de la empresa |
| `/servicios/administracion-deportiva` | Administración de escenarios |
| `/servicios/servicios-deportivos` | Servicios deportivos |
| `/servicios/servicios-recreativos` | Servicios recreativos |
| `/escenarios-deportivos` | Catálogo de escenarios |
| `/escenarios-deportivos/[id]` | Ficha individual de cada escenario |
| `/formacion` | Programas de formación |
| `/clientes` | Clientes y casos |
| `/unofit` | Línea de negocio UnoFit |
| `/contacto` | Formulario de contacto |

---

## ✨ Detalles de implementación

- **Rutas dinámicas** para las fichas de escenario (`[id]`), con estados de carga propios
  (`loading.tsx`) aprovechando el streaming del App Router.
- **Proveedor de animaciones** centralizado (`animation-provider.tsx`) para mantener una
  única configuración de transiciones en todo el sitio.
- **Botón flotante de WhatsApp** como canal principal de conversión.
- **Modo claro/oscuro** mediante `theme-provider`.

---

## 🧱 Stack

- **Next.js** (App Router) · **React** · **TypeScript**
- **Tailwind CSS** + **shadcn/ui** (Radix UI)
- **Framer Motion** — animaciones
- **next-themes** — tema claro/oscuro

---

## 🚀 Ejecutar

```bash
git clone https://github.com/SANTIAGORF24/sportsprofessionals.git
cd sportsprofessionals
pnpm install
pnpm dev       # http://localhost:3000
```

---

## 📂 Estructura

```
app/
├── page.tsx · layout.tsx
├── servicios/               tres líneas de servicio
├── escenarios-deportivos/   catálogo + ruta dinámica [id]
├── formacion/ · clientes/ · unofit/
├── quienes-somos/ · contacto/
components/
├── banner-slider.tsx · service-card.tsx
├── navbar.tsx · footer.tsx
├── whatsapp-button.tsx
├── animation-provider.tsx · theme-provider.tsx
└── ui/                      componentes shadcn/ui
```

---

## 👤 Autor

**Santiago Ramírez Forero** — Desarrollador Full Stack
[LinkedIn](https://www.linkedin.com/in/santiago-ramírez-forero) · [GitHub](https://github.com/SANTIAGORF24)
