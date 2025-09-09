
# Pokémon Static - Astro

Este proyecto es una aplicación web estática que muestra un listado de los primeros 151 Pokémon utilizando la [PokeAPI](https://pokeapi.co/). Está construido con [Astro](https://astro.build/) y utiliza [Tailwind CSS 4](https://tailwindcss.com/) para los estilos.

## 🚀 ¿Qué hace este proyecto?

- Muestra una lista de Pokémon con imágenes oficiales y enlaces a una página de detalle para cada uno.
- Cada página de detalle incluye información básica, imagen y el grito (audio) del Pokémon.
- El sitio es completamente estático y puede ser desplegado en cualquier hosting de archivos estáticos.

## �️ Tecnologías utilizadas

- **Astro**: Framework moderno para sitios web estáticos y rápidos.
- **Tailwind CSS 4**: Utilidad para estilos rápidos y personalizables.
- **TypeScript**: Tipado estático para mayor robustez.
- **PokeAPI**: API pública para obtener datos de Pokémon.

## 📁 Estructura del proyecto

```
/
├── public/                # Archivos estáticos (favicon, imágenes, etc)
├── src/
│   ├── components/        # Componentes reutilizables (ej: PokemonCard)
│   ├── interfaces/        # Tipos y contratos TypeScript para la API
│   ├── layouts/           # Layouts principales (ej: MainLayout)
│   ├── pages/             # Páginas del sitio (index, pokemons/[name])
│   ├── styles/            # Estilos globales (global.css)
│   └── consts/            # Constantes globales (site-info)
├── astro.config.mjs       # Configuración de Astro y plugins
├── tailwind.config.js     # Configuración de Tailwind (si existe)
├── package.json           # Dependencias y scripts
└── tsconfig.json          # Configuración de TypeScript
```

## ⚙️ Detalles técnicos

- El proyecto utiliza rutas estáticas generadas con Astro (`getStaticPaths`) para cada Pokémon.
- Los estilos se aplican usando clases de Tailwind directamente en los componentes y páginas.
- El layout principal importa los estilos globales y define metadatos para SEO y redes sociales.
- El consumo de la API se realiza en tiempo de build, por lo que el sitio es rápido y no depende de un backend propio.

## 🧞 Comandos útiles

Todos los comandos se ejecutan desde la raíz del proyecto:

| Comando           | Acción                                         |
|-------------------|-----------------------------------------------|
| `npm install`     | Instala las dependencias                      |
| `npm run dev`     | Inicia el servidor de desarrollo (`localhost:4321`) |
| `npm run build`   | Genera el sitio estático en `./dist/`         |
| `npm run preview` | Previsualiza el sitio generado                |

## 👨‍� Autor

David Ghiano

---

¿Dudas o sugerencias? ¡Abre un issue o contacta al autor!
