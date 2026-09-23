# ATELIER — Premium Fashion Design System

Design system premium para e-commerce de moda. HTML y CSS puro, sin frameworks, con tokens de diseño, componentes reutilizables y 23 templates de páginas listos para producción.

**Demo:** https://premium-fashion-design-system.vercel.app

## Qué incluye

- **23 templates de e-commerce** — home, category, product, cart, checkout, order-success, account, wishlist, login, contact, blog, 404 y más.
- **7 hojas de tokens** — colores, tipografía, espaciado, bordes, sombras, breakpoints y animaciones, centralizados en `tokens.css`.
- **13 componentes documentados** — buttons, cards, inputs, modals, navigation, product-cards, search-overlay, selectors, tooltips, feedback, badges, accordions.
- **CSS organizado por capas** — `tokens.css` · `base.css` · `components.css` · `responsive.css` · `dark-mode.css` · `accessibility.css`.
- **Dark mode y accesibilidad** contratados de forma progresiva.

## Estructura

```
├── tokens/          → Hojas de documentación de tokens (colors, typography, spacing, ...)
├── components/      → Documentación de componentes con ejemplos de uso
├── pages/           → 23 templates de e-commerce completos
└── assets/styles/   → CSS por capas: tokens, base, components, responsive, dark-mode, accessibility
```

## Cómo usarlo

```bash
# Ver las páginas
cd pages && python3 -m http.server 8080
# Abrir http://localhost:8080/home.html
```

1. Abre `tokens/colors.html` y `tokens/typography.html` para conocer el sistema de tokens (`--color-*`, `--font-*`, `--space-*`, `--radius-*`).
2. Usa los componentes de la carpeta `components/` como bloques ya resueltos (header, product cards, modales, formularios).
3. Copia la estructura de capas CSS de `assets/styles/` a tu proyecto.

## Principios de diseño

- Dirección de arte editorial: tipografía display expresiva, espaciado generoso y paleta neutra con acentos.
- Sin dependencias externas: todo el sistema corre sobre HTML/CSS vanilla.
- Accesibilidad: contraste AA, estados de foco visibles y markup semántico.
- Responsive mobile-first con breakpoints definidos por token.